# How Data Travels from Your Computer to a Website

Module: Hardware, Networks, and Behaviorist AI  
Audience: Beginners  
Content version: V1.0 
Status: Drafted — needs peer review and source verification

## Learning goals

After studying this topic, you should be able to:
- describe the purpose of DNS in a website visit;
- identify the roles of your device, local network, router, internet, and web server;
- put the main stages of a simplified website request in the correct order; and
- explain why the response must travel back to your browser.

## 1. The big idea

When you type a website name into a browser, your computer does not magically receive a page. Your browser and operating system use networking services to find the destination, send a request, and receive a response. The browser then interprets the returned web content and displays the page.

A **network** is a group of connected devices that can exchange data. Data is sent in units commonly called **packets** as it travels across many networks. A **server** is a computer or software system that provides a service—in this example, it sends website content when requested.

The exact route depends on the network and the website. The sequence below is a simplified learning model, not a promise that every request follows an identical path.

## 2. Key terms

| Term | Beginner-friendly meaning |
|---|---|
| Browser | An application used to request and display web pages, such as Chrome, Firefox, Safari, or Edge. |
| DNS (Domain Name System) | A distributed naming system that helps find the IP address associated with a domain name. |
| IP address | A logical network address used to deliver data to a destination across IP networks. |
| Router | A device that forwards packets between networks, such as a home network and an internet service provider's network. |
| Switch | A device that connects devices within a local wired network and forwards Ethernet frames toward the appropriate local connection. |
| Wi-Fi access point | A device that lets wireless devices connect to a local network. It may be built into a home router. |
| Server | A computer or software service that responds to requests, for example by providing web content. |
| Packet | A formatted unit of data carried by a network protocol. |
| Protocol | An agreed set of rules that devices use to communicate. |
| HTTPS | HTTP communication protected with TLS encryption and authentication. It helps protect data in transit between the browser and the website endpoint. |

## 3. The journey in a simplified diagram

```text
You enter a website name
          |
          v
Browser / operating system
          |
          |  DNS lookup: find an IP address
          v
DNS resolver (often provided by your network or chosen service)
          |
          v
Browser connects to the website's server
          |
          v
Local network: Wi-Fi access point or Ethernet switch
          |
          v
Router -> Internet service provider -> networks across the internet
          |
          v
Website server sends a response
          |
          v
Response returns through the network path
          |
          v
Browser processes the response and displays the page
```

**Important:** This diagram separates DNS from the website connection to make the ideas easier to learn. DNS information may already be cached, and the network path may include many routers. A home gateway may combine a router, switch, Wi-Fi access point, and other functions in one box.

## 4. Step-by-step worked example

Imagine that you type `https://www.example.com` into your browser. `example.com` is used here as an illustrative domain.

1. **You enter the address.** The browser interprets the address and identifies the website hostname.
2. **The browser needs an IP address.** Computers communicate over IP networks using IP addresses. The browser or operating system may already have a suitable DNS result in its cache.
3. **DNS resolution happens if needed.** A DNS resolver helps find the IP address associated with the hostname. DNS translates names to records; it does not download the web page itself.
4. **The browser establishes a connection.** For HTTPS, the browser typically establishes a secure connection with the server endpoint, using modern transport and security protocols. The exact details depend on the browser, server, and network.
5. **The browser sends a web request.** The request is carried in network data. Your device sends it over Wi-Fi or Ethernet to the local network and usually to a router that can forward it toward the internet.
6. **Networks forward the data.** Routers forward packets toward the destination. The data may pass through multiple networks and routers; there is not one universal route.
7. **The server responds.** The website service processes the request and sends a response, which can contain HTML and references to other resources such as stylesheets, scripts, and images.
8. **The browser displays the result.** The response returns across the network. The browser processes the received content and may make additional requests for the resources needed to render the page.

### What role does each component play?

- **CPU:** executes browser and operating-system instructions while the request is prepared and the page is processed.
- **RAM:** temporarily holds programs and data currently in use.
- **Network interface:** sends and receives network data over Ethernet or Wi-Fi.
- **Router:** forwards packets between networks.
- **DNS resolver:** helps resolve the domain name to an IP address.
- **Web server:** responds to the browser's request.

This example connects hardware and networking: the CPU and RAM help run the software, the network interface moves data, and network devices forward it toward the destination.

## 5. Check your understanding

### Activity A — Put the stages in order

Put these stages in an order for a simplified website visit:

- A. The browser processes the response and displays the page.
- B. The browser/operating system obtains an IP address, using DNS if needed.
- C. The browser sends a request toward the website server.
- D. The website server sends a response.
- E. You enter a website address.

**Your answer:** Write the letters in order and give one sentence explaining the role of DNS.

### Activity B — Apply the idea

A learner can connect to the home Wi-Fi network, but one website does not load. Give two safe, basic checks they could try before assuming that the router is broken.

## 6. Answers and explanations

**Activity A:** E → B → C → D → A.

- You enter the address first.
- The device obtains the destination IP address, unless a usable result is already cached.
- The browser sends a request; the server responds; then the browser processes the response.
- **DNS's role:** it helps translate a domain name into the IP address needed to contact the destination. DNS does not itself send the page content.

**Activity B — possible answers:**
1. Check whether other websites load. This helps determine whether the problem is limited to one website.
2. Check the address for typing mistakes and try reloading the page.
3. Check whether the device still has a working network connection.
4. If permitted by the household or school's rules, ask the network administrator or responsible adult before changing network settings or restarting shared equipment.

These are initial checks, not a guaranteed diagnosis. A site, DNS service, browser, device, or network may be responsible.

## 7. Mini-lecture plan (5–10 minutes)

1. **Hook (1 minute):** Ask, “What do you think happens after you type a website name and press Enter?”
2. **Introduce terms (2 minutes):** Explain DNS, IP address, router, and server using the table above.
3. **Walk through the diagram (3 minutes):** Trace the request from the browser to the server and the response back.
4. **Quick activity (2 minutes):** Ask learners to order Activity A and explain DNS.
5. **Exit question (1 minute):** “Does DNS download the website page?” Expected answer: no; it helps resolve the name to an address.

## 8. How this topic can become other learning resources

- **Study guide:** keep the key-term table, worked example, and activities with answers.
- **PPT slides:** use one slide for the diagram, one for the step-by-step journey, and one for the check-your-understanding activity.
- **Video tutorial:** narrate the diagram while highlighting each stage; finish with the ordering question.

## 9. References

1. Internet Engineering Task Force (IETF), **RFC 1034: Domain Names — Concepts and Facilities**. https://www.rfc-editor.org/rfc/rfc1034  
   Supports the role and general design of the Domain Name System.
2. Internet Engineering Task Force (IETF), **RFC 9110: HTTP Semantics**. https://www.rfc-editor.org/rfc/rfc9110  
   Supports the concepts of HTTP requests, responses, and semantics.
3. Internet Engineering Task Force (IETF), **RFC 8446: The Transport Layer Security (TLS) Protocol Version 1.3**. https://www.rfc-editor.org/rfc/rfc8446  
   Supports the description of TLS as a security protocol used to protect communication.
4. Cloudflare Learning Center, **What is a DNS server?** https://www.cloudflare.com/learning/dns/what-is-a-dns-server/  
   Provides a beginner-oriented explanation of DNS resolvers and name resolution.

**Source-use note:** The explanations above are paraphrased for beginner learners. Before submission, the team should open the sources, confirm that they support the statements, add any sources used for diagrams or images, and follow the course's attribution rules.
