# 🔢 Module 01: Number Systems & Digital Data Representation
### *How Computers Turn Voltage Switches into Numbers, Text, Photos, Music, and 4K Video*




---

## 🍌 Topic 1: Number Systems (Binary, Octal, Decimal & Hexadecimal)

### 💡 The Hook: Counting With 10 Fingers vs. Counting With Light Switches

Imagine you walk into a fruit market to count a basket of **apples and bananas**. Why do humans naturally group things into tens (`10, 100, 1000`)? Because we were born with **10 fingers**! That everyday system is called **Decimal (Base 10)**.

Now look inside your laptop's processor. A silicon chip does **not** have 10 fingers. Instead, it is built out of billions of microscopic electrical switches called **transistors**. A switch only knows two states:
* **OFF (`0`)** — Low voltage (~0.0V)
* **ON (`1`)** — High voltage (~1.0V)


*Real-World Binary in Action: The electronic binary clock at the St. Gallen railway station in Switzerland displays hours, minutes, and seconds purely using ON (`1`) and OFF (`0`) lights ([Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Binary_clock_Swiss_railway_station.jpg)).*


*Historical Milestone: Gottfried Wilhelm Leibniz's original 1703 manuscript showing how any decimal number can be represented using only `0` and `1` ([Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Leibniz_binary_system_1703.png)).*

> [!IMPORTANT]
> **⚡ Why Don't Engineers Build Base-10 Computers?**
> What if we tried to make a circuit where `0.1V = 1`, `0.2V = 2`, `0.3V = 3` ... up to `1.0V = 10`? Electrical wires heat up, batteries drain, and neighboring wires cause electromagnetic interference (*thermal noise*). At 3.5 billion ticks per second, `0.4V` would constantly blur into `0.5V`, corrupting your data! Using **Binary (Base 2)** gives hardware massive **noise immunity**: a transistor is unmistakably **OFF (`0`)** or **ON (`1`)**.

---

### 📐 1.1 Positional Notation: How Base 10, Base 2, Base 8, and Base 16 Work

In any **positional number system** with base $b$, there are exactly $b$ allowed symbols (from $0$ to $b-1$), and each column's weight is a power of $b$ from right to left:

$$\text{Value} = d_n \times b^n + \dots + d_2 \times b^2 + d_1 \times b^1 + d_0 \times b^0$$

| Number System | Base ($b$) | Allowed Symbols | Place Values (Right $\leftarrow$ Left) | Real-World Computing Use Cases |
| :--- | :---: | :--- | :--- | :--- |
| **Decimal** | **Base 10** | `0, 1, 2, 3, 4, 5, 6, 7, 8, 9` | $10^3=1000,\; 10^2=100,\; 10^1=10,\; 10^0=1$ | Everyday human math, IPv4 addresses (`192.168.1.10`) |
| **Binary** | **Base 2** | `0, 1` *(bits)* | $2^7=128,\; 2^6=64,\; 2^5=32,\; 2^4=16,\; 2^3=8,\; 2^2=4,\; 2^1=2,\; 2^0=1$ | All CPU registers, RAM capacitors, SSD flash cells, and network signals |
| **Octal** | **Base 8** | `0, 1, 2, 3, 4, 5, 6, 7` | $8^2=64,\; 8^1=8,\; 8^0=1$ *(1 octal digit = **3 bits**)* | Linux/Unix file permissions (`chmod 754` $\rightarrow$ `rwxr-xr--` = `111 101 100₂`) |
| **Hexadecimal** | **Base 16** | `0–9` and `A` (10), `B` (11), `C` (12), `D` (13), `E` (14), `F` (15) | $16^2=256,\; 16^1=16,\; 16^0=1$ *(1 hex digit = **4 bits**)* | Memory addresses (`0x0040A000`), Wi-Fi MAC addresses (`A4:83:E7:12:9B:04`), CSS RGB colors (`#FF8800`), IPv6 |


*Visual Analogy: Four binary switches (`0`/`1`) group neatly into one Hexadecimal digit (`0–F`) and encode pixels and sound waves.*

---

### 🔄 1.2 Step-by-Step Base Conversions & The 4-Bit "Nibble" Shortcut


*Schematic Breakdown: Converting the 8-bit byte `10101101₂` (Decimal `173`) into Hexadecimal `0xAD` in two seconds by splitting it into two 4-bit nibbles.*

Let's convert the number **`173`** across all four bases step by step:

1. **Binary $\rightarrow$ Decimal (Add the Active Powers of 2):**
   Write the 8-bit weights above the bits (`128, 64, 32, 16, 8, 4, 2, 1`) and sum every column that has a `1`:
   * For `10101101₂`:
   $$128 + 0 + 32 + 0 + 8 + 4 + 0 + 1 = \mathbf{173_{10}}$$

2. **Decimal $\rightarrow$ Binary (Largest Power Subtraction or Division by 2):**
   Subtract the largest powers of 2 that fit inside `173`:
   * $173 - 128 = 45$ (put `1` at 128)
   * $45 - 32 = 13$ (put `0` at 64, `1` at 32)
   * $13 - 8 = 5$ (put `0` at 16, `1` at 8)
   * $5 - 4 = 1$ (put `1` at 4, `0` at 2)
   * $1 - 1 = 0$ (put `1` at 1)
   * Result: **`10101101₂`**

3. **Binary $\leftrightarrow$ Hexadecimal (The 4-Bit Nibble Shortcut):**
   Because $16 = 2^4$, **every 4 binary bits (a *nibble*) map to exactly 1 Hexadecimal digit (`0–F`)!** You never need to divide by 16:
   * **Step 1:** Split the 8-bit byte `10101101₂` down the middle into two 4-bit nibbles: `1010` and `1101`.
   * **Step 2:** Score each nibble using weights `8, 4, 2, 1`:
     * Left nibble: `1010₂` = $8 + 0 + 2 + 0 = 10 = \mathbf{A_{16}}$
     * Right nibble: `1101₂` = $8 + 4 + 0 + 1 = 13 = \mathbf{D_{16}}$
   * **Step 3:** Combine them with the `0x` prefix: **`0xAD`**!
   * *Going backwards (Hex $\rightarrow$ Binary):* Expand each Hex digit into 4 bits (`0xF4` $\rightarrow$ `F = 1111`, `4 = 0100` $\rightarrow$ `11110100₂`).

4. **Binary $\leftrightarrow$ Octal (The 3-Bit Grouping Shortcut):**
   Because $8 = 2^3$, group binary bits in **sets of 3** from right to left using weights `4, 2, 1`:
   * `10101101₂` $\rightarrow$ `010` (`2`) | `101` (`5`) | `101` (`5`) = **`255₈`** ($2 \times 64 + 5 \times 8 + 5 \times 1 = 173_{10}$).

#### Why Hexadecimal Matters to Every Engineer
Try reading a 32-bit RAM address in raw binary: `00000000010000001010000000000000₂`. It is an eye-blurring wall of 32 digits! If you convert it to Decimal (`4,235,264`), you lose all visibility into which byte is which. **Hexadecimal** compresses every 8-bit byte into **2 clean characters (`0x00` to `0xFF`)**, turning that 32-bit address into **`0x0040A000`**.

#### Master 4-Bit Nibble Reference Table (`0` – `15`)

| Decimal | 4-Bit Binary | Octal | Hex | Decimal | 4-Bit Binary | Octal | Hex |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **0** | `0000` | `0` | **`0`** | **8** | `1000` | `10` | **`8`** |
| **1** | `0001` | `1` | **`1`** | **9** | `1001` | `11` | **`9`** |
| **2** | `0010` | `2` | **`2`** | **10** | `1010` | `12` | **`A`** |
| **3** | `0011` | `3` | **`3`** | **11** | `1011` | `13` | **`B`** |
| **4** | `0100` | `4` | **`4`** | **12** | `1100` | `14` | **`C`** |
| **5** | `0101` | `5` | **`5`** | **13** | `1101` | `15` | **`D`** |
| **6** | `0110` | `6` | **`6`** | **14** | `1110` | `16` | **`E`** |
| **7** | `0111` | `7` | **`7`** | **15** | `1111` | `17` | **`F`** |

> [!TIP]
> **🧠 Quick Practice Check:**
> * Convert `11001010₂` to Hex, Octal, and Decimal:
>   * **Hex:** `1100` (`12 = C`) + `1010` (`10 = A`) = **`0xCA`**
>   * **Octal:** `011` (`3`) + `001` (`1`) + `010` (`2`) = **`312₈`**
>   * **Decimal:** $128 + 64 + 8 + 2 = \mathbf{202_{10}}$
> * Decode Wi-Fi MAC prefix `A4:83` into binary:
>   * `A` (`1010`), `4` (`0100`), `8` (`1000`), `3` (`0011`) $\rightarrow$ **`10100100 : 10000011₂`**

---

## 🎨 Topic 2: Digital Data Storage & Representation (Numbers, Text, Images, Audio & Video)

### 💡 The Hook: Same Bits, Five Completely Different Meanings!

Suppose we look inside a computer's memory and find this single 8-bit byte:

$$\mathbf{\texttt{01000001}_2}$$

What is it?
* In a **calculator app**, it is the number **`65`**.
* In a **text editor**, it is the uppercase English letter **`'A'`**.
* In a **photo**, it is a dark shade of **Red (`65 / 255`)** inside one pixel.
* In a **music file**, it is the air-pressure height of a **sound wave** at one microsecond.

**How does the computer know which one it is?** The bits themselves carry no tags! The **file format and program context** (`.txt`, `.png`, `.mp3`, `.mp4`) tell the CPU how to interpret the binary stream.


*Complete Overview: How numbers, text, images, audio, and video are encoded into raw binary bits.*

---

### 🔢 2.1 Storing Numbers: Unsigned, Two's Complement & Floating-Point

1. **Unsigned Integers (Non-Negative Whole Numbers):**
   * All 8 bits in 1 byte represent positive magnitude from `00000000₂` (`0`) to `11111111₂` ($2^8 - 1 = 255$).
   * A 32-bit unsigned integer holds $0$ to $2^{32} - 1 = 4,294,967,295$ (~4.29 billion).

2. **Signed Integers (Two's Complement for Negative Numbers):**
   * How do we store `-5`? If we just used the first bit as a `-` sign (*sign-magnitude*), we would waste a pattern on `-0` (`10000000₂`) and need separate subtraction circuits.
   * Instead, every modern CPU uses **Two's Complement**: in an 8-bit signed byte (`-128` to `+127`), the leftmost bit has negative weight **`-128`** instead of `+128`.
   * **Shortcut to Negate Any Binary Number:** **Invert all bits (`0` $\leftrightarrow$ `1`) and add `1`!**
     * Start with $+5$: `00000101₂`
     * Invert all bits: `11111010₂`
     * Add `1`: **`11111011₂`** ($-128 + 64 + 32 + 16 + 8 + 2 + 1 = \mathbf{-5}$)
   * **Why CPUs Love It:** Add $+5 + (-5)$ using normal binary addition: `00000101 + 11111011 = 00000000` (`0`)! The CPU's standard addition circuit handles subtraction automatically.

3. **Real Numbers with Decimals (IEEE 754 Floating-Point):**
   * Fractional numbers like `-0.1` or $\pi = 3.14159$ are stored in binary scientific notation ($\pm 1.\text{Mantissa} \times 2^{\text{Exponent}}$) split into three fields:
     * **1 Sign Bit** (`0` = positive, `1` = negative)
     * **Exponent Bits** (moves the binary point left/right)
     * **Mantissa / Fraction Bits** (stores the significant digits)

---

### 📝 2.2 Storing Text: ASCII vs. Unicode (UTF-8)


*Standard 7-Bit ASCII Lookup Table mapping numbers `0–127` (`0x00–0x7F`) to English letters, digits, and control symbols ([Wikimedia Commons](https://commons.wikimedia.org/wiki/File:ASCII-Table.svg)).*

* **ASCII (American Standard Code for Information Interchange):**
  Uses 7 bits (stored in 1 byte) to map 128 English characters:
  * `'A'` = `65` (`0x41` = `01000001₂`)
  * `'a'` = `97` (`0x61` = `01100001₂`) — *Notice that lowercase is just uppercase + 32 (flipping 1 bit)!*
  * `'0'` = `48` (`0x30` = `00110000₂`)
* **Unicode & UTF-8 (Global Languages & Emojis):**
  One byte (256 values) is way too small for Indonesian, Japanese (`日本語`), Chinese (`汉字`), Arabic, math symbols, and emojis (`🚀`, `🤖`). Modern computers use **Unicode** encoded as **UTF-8**:
  * **100% backward-compatible with ASCII:** Standard English letters still take **1 byte**.
  * **Variable-length expansion:** International scripts use **2 or 3 bytes**, and emojis use **4 bytes**, supporting over 150,000 characters worldwide!

---

### 🖼️ 2.3 Storing Images: Bitmap Pixels (RGB) vs. Vector Math


*The 3D RGB Color Cube: Mixing Red, Green, and Blue light intensities from `0` to `255` (`0x00` to `0xFF`) creates $256^3 = 16,777,216$ distinct colors ([Wikimedia Commons](https://commons.wikimedia.org/wiki/File:RGB_color_cube.svg)).*

| Image Type | File Formats | How It Is Stored in Bits | What Happens When You Zoom In 1,000%? |
| :--- | :--- | :--- | :--- |
| **Bitmap (Raster)** | `.png`, `.jpg`, `.bmp`, `.webp` | A 2D grid of colored dots (**pixels**). In **24-bit True Color (RGB)**, each pixel uses **3 bytes**: 1 byte Red (`0–255`), 1 byte Green (`0–255`), 1 byte Blue (`0–255`). | Looks **blocky / pixelated** because the grid has a fixed number of pixels. |
| **Vector** | `.svg`, `.ai`, `.eps` | Stores **mathematical geometry formulas** (coordinates for lines, Bézier curves, circles, and fill colors). | Stays **100% razor-sharp at any size** because the computer recalculates the math on the fly! |

---

### 🎵 2.4 Storing Audio: Sampling Rate & Bit Depth (PCM)


*Digital Audio Sampling (PCM): An analog sound wave (red curve) is measured at fixed time intervals (**Sampling Rate** on the horizontal axis) and rounded to binary steps (**Bit Depth / Quantization** on the vertical axis) ([Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Pcm.svg)).*


*Side-by-Side Comparison: How a 24-bit RGB color (`#2B7A78`) splits into 3 bytes (left) and how an Analog-to-Digital Converter (ADC) samples a continuous sound wave (right).*

Sound in the air is a continuous analog pressure wave. A microphone's **Analog-to-Digital Converter (ADC)** converts it into binary using two parameters:
1. **Sampling Rate (measured in Hz / kHz):** How many times per second we measure the wave's height. CD-quality audio uses **`44.1 kHz`** (44,100 samples per second per channel). Higher sampling rates capture higher-pitched treble frequencies accurately.
2. **Bit Depth (e.g., 16-bit or 24-bit):** How many bits are used to record each sample's vertical height. A 16-bit sample provides $2^{16} = 65,536$ vertical levels, eliminating background quantization hiss.

---

### 🎬 2.5 Storing Video: Frame Rate (FPS) & Spatial/Temporal Codecs

A digital video is a synchronized audio track paired with a fast flipbook of bitmap images called **frames**, shown at **24, 30, or 60 Frames Per Second (FPS)**.

* **Why Uncompressed Video Is Massive:**
  One 1080p frame ($1920 \times 1080$ pixels $\times$ 3 bytes RGB) is `~6.22 MB`. At 30 FPS, raw video consumes:
  $$6.22\text{ MB} \times 30\text{ FPS} \approx \mathbf{186.6\text{ MB per second}} \quad (\text{over } \mathbf{11\text{ GB per minute!}})$$
* **How Video Codecs (`H.264 / H.265 / AV1`) Shrink It by 98%:**
  1. **Spatial Compression (Within a Frame):** Groups matching color regions inside a single frame (like a blue sky or white wall), just like JPEG image compression.
  2. **Temporal Compression (Across Frames):** Instead of saving 30 full photos every second, the codec saves an occasional full **Keyframe (I-frame)** and then only records **the pixels that moved or changed** in the frames in between!
