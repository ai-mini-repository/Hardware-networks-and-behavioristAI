# ✦ LAB 404 MODULE 01: OVERVIEW, NUMBER SYSTEMS & DIGITAL DATA REPRESENTATION ✦
*Part A (`Sections A.0A – A.0B`) • Binary, Octal, Decimal, Hexadecimal & How Numbers, Text, Images, Audio, and Video Are Stored as Bits*





---

# ✦ THE CHRONICLES OF LAB 404 ✦
### **An Interactive Illustrated GitHub Field Manual, Hands-On Simulator Companion & Deep-Dive Case Book**
#### *Module: Computer Hardware, Packet Networks, and Behaviorist AI*








*Step inside the silicon workshop of CPUs, RAM, and UEFI startup; follow packets across switches, routers, DNS, and stateful firewalls; and train behaviorist AI agents through rewards, penalties, and interactive labs.*

**Guided by:** `Dr. Ada Lin` (Chief Systems Architect) • `Byte, Unit B-04` (Apprentice Robot Agent) • `Inspector Ping` (Diagnostics & Security Detective)

---

---

## 🧭 Welcome to Lab 404: Explorer's Guide & Learning Route

Welcome, apprentice engineer! You have just stepped inside **Computing Laboratory 404**—an underground research workshop where silicon hardware, global packet networks, and behaviorist learning robots come alive. Unlike a passive textbook designed for memorizing dry definitions before an exam, this repository is an **active field manual**. Across every section, you will encounter a real-world mystery, record your prediction *before* seeing the outcome, run an experiment on paper or in a live browser simulator, and test why the underlying ideas matter in the real world.

| Explorer Guide Field | What You Will Master in This Repository |
| :--- | :--- |
| **Repository Title** | *The Chronicles of Lab 404: Exploring Hardware, Networks & Behaviorist AI* |
| **Module Scope** | **Part A:** Computer Hardware (`A.0A`–`A.VI`) • **Part B:** Computer Networks (`B.I`–`B.VII`) • **Part C:** Behaviorist AI (`C.I`–`C.VIII`) • **Part F:** Deep-Dive Case Files & Extra-Credit Python Maze Suite (`F.1`–`F.5`) • **Part E:** Master Glossary, Comparison Cards, Checklist & Bibliography (`E.1`–`E.4`) |
| **Target Audience & Prerequisites** | First-year computing beginners. Assumed prerequisites: basic everyday familiarity with opening desktop/mobile apps, saving files, and browsing the web. **Zero prior programming or electronics training required.** |
| **How to Use This Manual** | Read each subtopic's mystery challenge, write your prediction before checking the explanation, try the hands-on simulators, and verify your mastery with the 22 Detective Case Files and Self-Check Reviews! |

### 👥 Meet Your Recurring Guides in Lab 404


***Figure 0.1 — Lab 404 Field Team:** Dr. Ada Lin, Byte (Unit B-04), and Inspector Ping's diagnostic lens.*

Throughout this learning material, three recurring characters accompany your investigations across schematics, videos, interactive activities, and detective cases so that every chapter feels like a connected story:

* 👩‍🔬 **Dr. Ada Lin (Chief Systems Architect):** The calm, sharp-witted founder of Lab 404. Whenever a concept seems mysterious—like why RAM loses your essay when the power cord trips, or how a CPU executes billions of instructions per second—Dr. Lin steps in to connect everyday metaphors to accurate technical architecture without oversimplifying the truth.
* 🤖 **Byte, Unit B-04 (Apprentice Robot Agent):** A curious, literal-minded wheeled robot built in Lab 404. In **Part A**, Byte's onboard processor and memory chips are our patient under the microscope. In **Part B**, Byte tries to send telemetry packets across the lab's Local Area Network. In **Part C**, Byte becomes our reinforcement learning test subject—navigating grid-world mazes and occasionally finding hilarious loopholes whenever we design a sloppy reward function.
* 🕵️‍♂️ **Inspector Ping (Diagnostics & Security Detective):** Lab 404's resident network sleuth. Inspector Ping has one strict rule: *never say "the computer is broken" or "the internet is down" when you can record an exact observation.* He guides our troubleshooting checklists, packet traces, and firewall rule-table evaluations.

### 🗺️ Complete Module Curriculum & Pacing Map

| Part / Section | Core Topic & Embedded Hands-On Investigations | Suggested Pace |
| :--- | :--- | :---: |
| **Front Matter** | Identification, Cast of Characters, Learning Goals, 6-Step Inquiry Cycle & Study Route | `15 mins` |
| **Part A: Hardware**
`Section A.0A` | **Number Systems (Binary, Octal, Decimal & Hexadecimal):** Positional Notation, Why Computers Use Binary, Step-by-Step Base Conversions, the 4-Bit Nibble Shortcut & Why Hexadecimal Matters | `40 mins` |
| `Section A.0B` | **Digital Data Storage & Representation:** How Numbers (Unsigned, Two's Complement, Floating-Point), Text (ASCII & UTF-8/Unicode), Images (RGB Pixels & Vectors), Audio (Sampling & Bit Depth) & Video (FPS & Codecs) Are Stored as Bits | `40 mins` |
| `Section A.I` | **Core Components & Von Neumann Model:** Inside the CPU (ALU, Control Unit, Registers, Cache), Fetch–Decode–Execute Cycle, Motherboard Buses, GPU Parallelism, Power & Cooling | `45 mins` |
| `Section A.II` | **RAM vs. Storage:** Volatility vs. Persistence, DRAM Capacitors vs. NAND Flash & Magnetic Platters, Memory Hierarchy Latency Scale, Virtual Memory & Paging | `40 mins` |
| `Section A.III` | **How a Computer Starts Up:** Power-On to Sign-In, UEFI vs. Legacy BIOS, POST, Firmware Boot Manager vs. OS Bootloader, Kernel, Drivers, Secure Boot & Network Boot | `45 mins` |
| `Section A.IV` | **What Happens When You Open an Application:** OS Process Creation, Virtual Address Space, RAM Working Buffers, Saving Files to Storage & Local vs. Online Tasks | `40 mins` |
| `Section A.V` | **How the Components Work Together:** Address/Data/Control Buses, Hardware Interrupts, Direct Memory Access (DMA), Bottlenecks & Full System Traces | `35 mins` |
| `Section A.VI` | **Hardware Activities & Platform Labs:** Little Man Computer (LMC) CPU Lab, Human Motherboard Card Game, Live Process/RAM Experiment, Startup Case Files & Review | `60 mins` |
| **Part B: Networks**
`Section B.I` | **Network Fundamentals and Types:** Packets & Frames, Bandwidth vs. Latency, PAN/LAN/WLAN/MAN/WAN, Client–Server vs. P2P & Network Topologies | `35 mins` |
| `Section B.II` | **Network Devices and Transmission Media:** NICs, Layer-2 Switches, Wireless Access Points, Layer-3 Routers, Home Gateways, Copper, Fiber-Optic & Wi-Fi Radio | `40 mins` |
| `Section B.III` | **Addresses and Protocols:** IPv4/IPv6, Subnet Masks, Private IPs (RFC 1918) & NAT, MAC Addresses, ARP, DHCP (DORA), DNS, TCP/IP Suite, TCP vs. UDP & HTTPS/TLS | `50 mins` |
| `Section B.IV` | **How Data Travels from Your Computer to a Website:** Step-by-Step 8-Stage Packet Journey, Local LAN Printing vs. Remote Web Requests & Hardware Synergy | `45 mins` |
| `Section B.V` | **Firewalls:** Host vs. Network Firewalls, 5-Tuple Packet Filtering, Top-Down Rule Evaluation, Implicit Deny, Stateful Inspection & Security Limits | `45 mins` |
| `Section B.VI` | **Basic Safety and Troubleshooting:** Evidence-Based Diagnostics, Separating Observation from Diagnosis, Safe CLI Tools (`ping`, `nslookup`) & Incident Reports | `35 mins` |
| `Section B.VII` | **Network Activities & Platform Labs:** Local Network Printer & ARP Lab, Packet Lantern Relay Game, Firewall Gatekeeper Lab, Browser DevTools Lab & Review | `60 mins` |
| **Part C: Behaviorist AI**
`Section C.I` | **What Is Behaviorist AI:** Psychological Behaviorism (Thorndike, Skinner) vs. Computational Reinforcement Learning; Symbolic, Statistical & Behaviorist Paradigms | `35 mins` |
| `Section C.II` | **The Agent–Environment Loop:** Agent, Environment, State vs. Observation, Action Space, Numerical Reward, Markov Decision Processes, Policy & Value Functions | `40 mins` |
| `Section C.III` | **Learning from Rewards and Penalties:** Trial-and-Error, Temporal Credit Assignment, Discount Factor, Exploration vs. Exploitation & Worked Grid-World Q-Learning Trace | `50 mins` |
| `Section C.IV` | **Reward Design:** Goal Rewards, Step Penalties, Obstacle Penalties, Reward Hacking / Specification Gaming Case Studies & Multi-Environment Testing | `40 mins` |
| `Section C.V` | **Rule-Based Systems vs. Learning Agents:** Fixed Rules & Prolog Knowledge Bases vs. Adaptive RL Policies, Hybrid Safety Systems & ELIZA Pattern Matching | `45 mins` |
| `Section C.VI` | **Applications and Limitations:** Robotics, Games, Data Centers, RLHF; Sample Inefficiency, Unsafe Physical Exploration & Sim-to-Real Transfer Gaps | `35 mins` |
| `Section C.VII` | **Common Misunderstandings:** Debunking 7 Persistent Myths About Rewards, Feedback, Memory, and Machine Understanding | `30 mins` |
| `Section C.VIII` | **Behaviorist AI Activities & Platform Labs:** Tabletop Q-Learning Lab, SWISH Prolog Lab, ELIZA Breakdown Lab, TensorFlow Playground, ML for Kids & River-Crossing Lab | `75 mins` |
| **Part F: Deep Dives**
`Sections F.1–F.5` | **Deep-Dive Case Files & Extra-Credit Robot Maze Suite:** Virtual Memory Page Fault Trace, Subnet Mask & NAT Math, Runnable Python Maze Suite, Cheat Cards & 22 Mystery Cases | `60 mins` |
| **Part E: Reference**
`Sections E.1–E.4` | **Master Glossary, Rapid-Fire Concept Comparison Cards, Self-Study Checklist & Technical Bibliography** | `Reference` |

### 🎯 Master Learning Goals & The 6-Step Active Inquiry Cycle

By working through the explanations, predictions, and hands-on missions in this repository, you will be able to:

1. **Trace Hardware Execution (Part A):** Explain the distinct roles of the CPU, motherboard, RAM, persistent storage, GPU, firmware (UEFI), bootloader, and OS kernel during both computer startup and everyday application execution, including why unsaved work in volatile RAM vanishes upon power loss.
2. **Follow Network Packets & Boundaries (Part B):** Distinguish local area communication (switches, wireless access points, MAC addresses, ARP, DHCP) from wide area routing (routers, IP addresses, DNS, TCP/IP, HTTPS/TLS), and evaluate how host and network firewalls filter traffic using top-down rule tables and stateful connection tracking.
3. **Analyze & Design Behaviorist AI Systems (Part C):** Formulate simple tasks using the agent–environment loop (observations, actions, rewards, penalties, policies), trace how trial-and-error learning updates action choices, diagnose perverse incentives in poorly designed reward functions, and contrast learning agents with fixed rule-based systems.
4. **Diagnose Systems Scientifically (Across All Parts):** Separate concrete, observable evidence from unsupported assumptions when troubleshooting startup failures, local printer issues, unreachable websites, or misbehaving AI agents.

> [!NOTE]
> **🔬 The 6-Step Active Inquiry Cycle Used in Every Chapter**
> 1. **Encounter a Challenge:** A real-world mystery in Lab 404 that cannot be solved by guessing.
> 2. **Predict & Try:** A pause point where you write down your intuition *before* reading the technical explanation.
> 3. **Observe the System:** A concrete worked trace, table, or diagram showing what happens inside the machine or network.
> 4. **Explain the Mechanism:** Beginner-friendly, technically accurate depth connecting hardware, protocols, or algorithms.
> 5. **Apply in a Hands-On Activity:** Structured experiments specifying *Goal*, *Preparation*, *Task*, *Observation*, *Reflection*, and *Feedback*.
> 6. **Check Understanding:** Immediate self-test questions with explained answers and diagnostic hints.

---

## 🔢 Section A.0A: Number Systems — Binary, Octal, Decimal, and Hexadecimal

### 1. Encounter the Challenge: Why Do Engineers Write Memory & MAC Addresses in Strange Letters Like `0xA4F0`?

Apprentice Leo opens Lab 404's system debugger and network inspector. Instead of ordinary everyday numbers, he sees RAM addresses written as `0x0040A000`, Wi-Fi hardware MAC addresses written as `A4:83:E7:12:9B:04`, and web page colors written as `#1B365D`. Meanwhile, Byte insists that deep inside his silicon chips, there are no letters or `0–9` digits at all—only `0` and `1`!


***Figure A.0a — From Switches to Hex & Media:** Four binary switches (`0`/`1`) group neatly into one Hexadecimal digit (`0–F`) and encode pixels and sound waves.*

To understand how hardware and networks operate, we must answer four foundational questions:
1. **What is a number system?**
2. **Why do computers use binary (`0` and `1`)?**
3. **How do we convert numbers between Binary, Octal, Decimal, and Hexadecimal?**
4. **Why is the Hexadecimal system so important?**

### 2. What Is a Positional Number System? (Decimal, Binary, Octal, and Hexadecimal)

A **positional number system** represents quantities using a chosen **base (or radix, $b$)**. In any base $b$, there are exactly $b$ unique digit symbols (from $0$ to $b-1$), and the value of each digit depends on its *position* (power of $b$) from right to left:

$$	ext{Value} = d_n 	imes b^n + \dots + d_1 	imes b^1 + d_0 	imes b^0$$

| Number System | Base ($b$) | Allowed Digit Symbols | Positional Place Values (Right to Left) | Where It Is Used in Computing |
| :--- | :---: | :--- | :--- | :--- |
| **Decimal** | **Base 10** | `0, 1, 2, 3, 4, 5, 6, 7, 8, 9` | $10^3=1000,\; 10^2=100,\; 10^1=10,\; 10^0=1$ | Everyday human counting, IPv4 dotted-quad bytes (`192.168.1.10`) |
| **Binary** | **Base 2** | `0, 1` *(called bits)* | $2^7=128,\; 2^6=64,\; 2^5=32,\; 2^4=16,\; 2^3=8,\; 2^2=4,\; 2^1=2,\; 2^0=1$ | All physical CPU transistors, DRAM capacitors, SSD cells, and wire signals |
| **Octal** | **Base 8** | `0, 1, 2, 3, 4, 5, 6, 7` | $8^2=64,\; 8^1=8,\; 8^0=1$ *(1 octal digit = **3 bits**)* | Linux/Unix file permissions (e.g., `chmod 754` = `111 101 100₂`) |
| **Hexadecimal** | **Base 16** | `0–9` plus `A` (10), `B` (11), `C` (12), `D` (13), `E` (14), `F` (15) | $16^2=256,\; 16^1=16,\; 16^0=1$ *(1 hex digit = **4 bits**)* | RAM addresses (`0x40A0`), MAC addresses (`A4:83...`), IPv6, RGB colors (`#FF8800`) |

> [!IMPORTANT]
> **⚡ Why Do Computers Use Binary (Base 2) Physically?**
> Why didn't engineers build CPUs using Base-10 circuits with ten different voltage levels (`0.1V, 0.2V, ..., 1.0V`)? Because electrical wires and microscopic transistors experience thermal noise and voltage drops! Distinguishing ten tiny voltage steps at 3.5 billion times per second would cause constant bit errors. By using **Binary (Base 2)**, a transistor only needs two unmistakable states: **OFF / Low Voltage (`0`)** and **ON / High Voltage (`1`)**, giving silicon hardware massive noise immunity and reliability.

### 3. How Do We Convert Between Number Systems? (Worked Step-by-Step Rules)


***Figure A.0a-2 — The 4-Bit Nibble Shortcut:** Grouping an 8-bit byte into two 4-bit nibbles converts Binary to Hexadecimal (`0xAD`) at a glance.*

Because $8 = 2^3$ and $16 = 2^4$ are exact powers of 2, converting between **Binary, Octal, and Hexadecimal** does not even require long division! Let's master all four conversions using the 1-byte example **Decimal `173`** shown in the schematic above:

1. **Binary $
ightarrow$ Decimal (Sum the Active Powers of 2):**
   Write the powers of 2 above each bit (`128, 64, 32, 16, 8, 4, 2, 1`) and add the positions where the bit is `1`:
   For `10101101₂`, we add $128 + 32 + 8 + 4 + 1 = \mathbf{173_{10}}$.
2. **Decimal $
ightarrow$ Binary (Subtraction or Remainder Method):**
   Subtract the largest powers of 2 that fit into `173`:
   $173 - 128 = 45;\; 45 - 32 = 13;\; 13 - 8 = 5;\; 5 - 4 = 1;\; 1 - 1 = 0$.
   Putting `1`s at `128, 32, 8, 4, 1` and `0`s elsewhere gives **`10101101₂`**! *(Equivalently, divide by 2 repeatedly and read the remainders bottom-to-top.)*
3. **Binary $\leftrightarrow$ Hexadecimal (The 4-Bit "Nibble" Shortcut — Why It Works!):**
   Because $2^4 = 16$, **every group of 4 binary bits (called a *nibble*, ranging from `0000₂ = 0` to `1111₂ = 15 = F`) corresponds to exactly ONE Hexadecimal digit!** To convert `10101101₂` to Hexadecimal:
   * **Step 1:** Split the 8-bit byte into two 4-bit nibbles: `1010` and `1101`.
   * **Step 2:** Convert each 4-bit group independently using weights `8, 4, 2, 1`:
     `1010₂` = $8 + 2 = 10 = \mathbf{A_{16}}$, and `1101₂` = $8 + 4 + 1 = 13 = \mathbf{D_{16}}$.
   * **Step 3:** Combine them: `10101101₂` = **`0xAD`**! *(The prefix `0x` tells programmers and assemblers the number is written in Base 16.)* Going from Hex back to Binary is just as fast: expand each Hex digit into its 4 bits (`0xF4` $
ightarrow$ `F = 1111`, `4 = 0100` $
ightarrow$ `11110100₂`).
4. **Binary $\leftrightarrow$ Octal (The 3-Bit Grouping Shortcut):**
   Because $2^3 = 8$, group binary bits in **sets of 3** from right to left (`4, 2, 1`): `10101101₂` splits as `010 101 101₂` = **`255₈`** ($2 	imes 64 + 5 	imes 8 + 5 	imes 1 = 173_{10}$).

#### Why Is the Hexadecimal System So Important?
Reading or typing a 32-bit memory address in raw binary (`00000000010000001010000000000000₂`) is exhausting and error-prone for humans, while converting 32 bits into Decimal (`4,235,264`) hides the underlying byte boundaries! **Hexadecimal is the universal shorthand of computer engineering** because it compresses every 8-bit byte into **exactly 2 readable characters (`0x00` to `0xFF`)** while preserving exact bit alignment (`0x0040A000`).

#### Master 4-Bit Nibble Conversion Table (`0` to `15`)

| Decimal (Base 10) | 4-Bit Binary (Base 2) | Octal (Base 8) | Hexadecimal (Base 16) | Decimal (Base 10) | 4-Bit Binary (Base 2) | Octal (Base 8) | Hexadecimal (Base 16) |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **0** | `0000` | `0` | **`0`** | **8** | `1000` | `10` | **`8`** |
| **1** | `0001` | `1` | **`1`** | **9** | `1001` | `11` | **`9`** |
| **2** | `0010` | `2` | **`2`** | **10** | `1010` | `12` | **`A`** |
| **3** | `0011` | `3` | **`3`** | **11** | `1011` | `13` | **`B`** |
| **4** | `0100` | `4` | **`4`** | **12** | `1100` | `14` | **`C`** |
| **5** | `0101` | `5` | **`5`** | **13** | `1101` | `15` | **`D`** |
| **6** | `0110` | `6` | **`6`** | **14** | `1110` | `16` | **`E`** |
| **7** | `0111` | `7` | **`7`** | **15** | `1111` | `17` | **`F`** |

### 4. Hands-On Activity A0-1: The "IM Hexa" Nibble & Address Decoder Lab

* **Goal:** Master fast mental conversions between Binary, Decimal, Octal, and Hexadecimal and decode real MAC addresses and RGB color bytes.
* **Preparation:** Paper, pencil, and the 4-bit Nibble Lookup Table above (plus optional Python terminal check: `bin(173), oct(173), hex(173)`).
* **Task:**
  1. Convert the 8-bit binary byte `11001010₂` into (a) Hexadecimal using the 4-bit nibble split, (b) Octal using the 3-bit split, and (c) Decimal.
  2. Byte's Wi-Fi NIC MAC address starts with `A4:83`. Convert both Hex bytes into 16 binary bits.
  3. Explain why converting a 16-bit binary value into Hexadecimal takes 10 seconds by grouping 4 bits, whereas converting it into Decimal requires adding up to 16 powers of 2.

> **✅ Click to Reveal Observation & Checked Feedback (Activity A0-1)**
>
> * **(1)** Splitting `1100 1010₂` into nibbles gives `1100₂ = 12 = C` and `1010₂ = 10 = A` $
> ightarrow$ **`0xCA`**. Grouping by 3 bits (`011 001 010₂`) gives **`312₈`**. Summing powers of 2 ($128 + 64 + 8 + 2$) gives **`202₁₀`**.
> * **(2)** `A4:83` in binary is **`10100100 : 10000011₂`** (`A=1010`, `4=0100`, `8=1000`, `3=0011`).
> * **(3)** Because $16 = 2^4$, each hexadecimal digit maps strictly to an isolated 4-bit boundary without carry-over across nibbles, whereas Base 10 ($10 
> eq 2^k$) cuts across binary bit positions and requires summing all active powers of 2.

---

---

## 🎨 Section A.0B: Digital Data Storage & Representation — Numbers, Text, Images, Audio, and Video

### 1. Encounter the Challenge: If RAM and SSDs Only Hold `0`s and `1`s, How Do They Store Photos, Songs, and Movies?

Byte opens five files on his laptop: a calculator spreadsheet (`numbers`), a Markdown study guide (`text`), a team photo (`image`), a voice recording (`audio`), and a lecture clip (`video`). Every single one of those files is stored on the SSD as a stream of `0`s and `1`s! How does the computer know whether the byte `01000001₂` means the number `65`, the capital letter `'A'`, a dark shade of red in a photo, or a quiet moment in a song?

> *"The bits themselves don't carry tags, Byte! The **context and file format** tell the CPU and software how to interpret each group of bits. Let's inspect how all five data types are encoded into binary."* — **Dr. Ada Lin**


***Figure A.0b — Overview of Digital Data Representation:** How integers/floats, ASCII/UTF-8 text, RGB pixel grids, sampled audio waveforms, and compressed video frames map onto binary bits.*

### 2. Deep-Dive Explanation: How Five Core Data Types Are Stored in Binary

#### 1. Storing Numbers: Unsigned Integers, Two's Complement Negative Numbers & Floating-Point
* **Unsigned Integers:** When storing non-negative whole numbers in 1 byte (8 bits), all 8 bits represent magnitude from `00000000₂` (`0`) to `11111111₂` ($2^8 - 1 = 255$). A 32-bit unsigned integer stores up to $2^{32} - 1 pprox 4.29	ext{ billion}$.
* **Signed Integers (Two's Complement):** How do computers store negative numbers like `-5`? Early engineers tried using the leftmost bit as a simple minus sign (*sign-magnitude*), but that created two zeros (`+0` and `-0`) and required complicated subtraction circuitry. Modern CPUs use **Two's Complement**: in an 8-bit signed byte, the leftmost bit has weight **$-128$** instead of $+128$ (covering $-128$ to $+127$). To negate any binary number in Two's Complement, you simply **invert all the bits (`0` $\leftrightarrow$ `1`) and add `1`**!
  * *Worked Example:* $+5 = 	exttt{00000101}_2 
ightarrow 	ext{invert } 	exttt{11111010}_2 + 1 = \mathbf{	exttt{11111011}_2 = -5}$ ($-128 + 64 + 32 + 16 + 8 + 2 + 1 = -5$).
  * *Hardware Advantage:* When the ALU adds $+5 + (-5)$ (`00000101 + 11111011`), ordinary binary addition naturally produces `00000000` (`0`, discarding carry) using the exact same adder hardware!
* **Real Numbers with Decimals (IEEE 754 Floating-Point):** Numbers with fractional parts (like reinforcement learning reward `-0.1` or $\pi = 3.14159$) are stored in binary scientific notation ($\pm 1.	ext{Mantissa} 	imes 2^{	ext{Exponent}}$) split across three bit fields: **1 Sign bit**, **Exponent bits**, and **Mantissa (Fraction) bits**.

#### 2. Storing Text: From ASCII to Unicode & UTF-8
* **ASCII (American Standard Code for Information Interchange):** Maps 128 basic English characters, digits, and punctuation marks to 7-bit numbers (`0–127`, stored in 1 byte): for example, uppercase `'A' = 65 (0x41 = 01000001₂)`, lowercase `'a' = 97 (0x61 = 01100001₂)`, and digit character `'0' = 48 (0x30)`.
* **Unicode & UTF-8:** Because 1 byte (256 values) cannot hold Chinese (`没事`), Japanese, Arabic, mathematical symbols, and emojis (`🤖`), modern systems use **Unicode** encoded as **UTF-8**. UTF-8 is backward-compatible with ASCII (1 byte per English letter) and smoothly expands to 2, 3, or 4 bytes for over 150,000 international characters!

#### 3. Storing Images: Bitmap Pixels (RGB) vs. Vector Geometry


***Figure A.0b-2 — Pixels & Sound Waves:** Left: A 24-bit RGB color (`#2B7A78`) split into 3 bytes. Right: Sampling an analog audio wave at discrete time ticks.*

* **Bitmap (Raster) Images (`.png`, `.jpg`, `.bmp`):** Stored as a 2D grid of microscopic colored dots called **pixels** (*picture elements*). In standard **24-bit True Color (RGB)**, each pixel uses **3 bytes (24 bits)**: 1 byte for **Red** (`0–255` or `0x00–0xFF`), 1 byte for **Green** (`0–255`), and 1 byte for **Blue** (`0–255`), mixing $256^3 = 16,777,216$ distinct colors!
* **Vector Images (`.svg`):** Instead of storing millions of individual pixels, vector files store mathematical formulas for lines, curves, and polygons—allowing diagrams and logos to scale to any screen size without ever becoming blurry or pixelated!

#### 4. Storing Audio: Sampling Rate and Bit Depth
Sound in the air is a continuous analog pressure wave. To store sound digitally, a microphone's **Analog-to-Digital Converter (ADC)** measures the wave's height at thousands of evenly spaced time ticks per second (**Sampling**) and rounds each measurement to a binary number (**Quantization**):
* **Sampling Rate (measured in Hertz, Hz / kHz):** How many samples are recorded per second (e.g., CD-quality audio uses `44.1 kHz` = 44,100 samples per second per channel). Higher sampling rates capture higher-pitched frequencies accurately.
* **Bit Depth (e.g., 16-bit or 24-bit):** How many bits are used to store each single sample ($2^{16} = 65,536$ vertical amplitude levels), reducing background quantization hiss.

#### 5. Storing Video: Frame Rate (FPS) and Compression Codecs
A digital **video** combines a synchronized audio stream with a rapid sequence of bitmap images called **frames** displayed at **24, 30, or 60 Frames Per Second (FPS)**. Because an uncompressed 1080p video at 30 FPS would consume $1920 	imes 1080 	imes 3	ext{ bytes} 	imes 30 pprox 186	ext{ MB per second}$ (over 11 GB per minute!), video formats (`MP4 / H.264 / H.265`) use two forms of compression:
* **Spatial Compression:** Grouping similar color blocks inside a single frame (like JPEG).
* **Temporal Compression:** Storing a full *keyframe* only occasionally and recording only the pixels that *moved or changed* in the frames between!

---

---
