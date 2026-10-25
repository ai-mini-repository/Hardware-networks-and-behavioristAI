# Module Outline: Hardware, Networks, and Behaviorist AI

**Status key:** `Outline only` = planned but not fully written; `Drafted` = initial substantive content exists; `Needs review` = a team member must check it; `Checked` = reviewed and the outcome recorded.

## Intended learners and prerequisites
- **Audience:** beginners with basic computer literacy.
- **Prerequisites:** ability to use a computer and a web browser; no prior hardware assembly, network configuration, or AI development experience is required.
- **Teaching approach:** plain-language explanations, labelled diagrams, everyday examples, short checks for understanding, and step-by-step examples of a website request and a behaviorist AI system.

## Intended learning outcomes
By the end of the module, learners should be able to:

1. Identify the CPU, motherboard, RAM, storage, and input/output devices and describe their basic roles.
2. Explain how major hardware components work together during a common computer task.
3. Distinguish volatile memory (RAM) from non-volatile storage (such as an SSD or HDD).
4. Distinguish PAN, LAN, WLAN, MAN, and WAN at an introductory level.
5. Describe the roles of a network interface card (NIC), switch, router, modem/ONT, and wireless access point.
6. Compare wired Ethernet and wireless Wi-Fi as ways to connect devices.
7. Explain, at a beginner level, the roles of IP addresses, MAC addresses, DNS, and TCP/IP.
8. Trace the main stages of a browser requesting a website, while recognizing that real network paths vary.
9. Identify a few safe, basic troubleshooting checks, such as checking Wi-Fi status and restarting an application or router when appropriate.
10. Explain the basic principles of behaviorist AI, including stimulus, response, feedback, and reward or penalty.
11. Describe how an AI agent can learn or adjust its behavior through interactions with an environment and feedback.
12. Distinguish a simple rule-based response system from a system that improves its behavior through experience.
13. Identify a basic application of behaviorist AI, such as an agent learning to navigate a simple environment or a game character adapting its actions based on rewards.

## Learning sequence and development status

| Order | Topic and subtopics | Planned example / activity | Status |
|---|---|---|---|
| 1 | Introduction to computer hardware and networks | Sort everyday items into hardware, software, and network components | Outline only |
| 2 | Core hardware: CPU, motherboard, RAM, storage, input/output | Match component names to roles; compare RAM with SSD storage | Outline only |
| 3 | How hardware works together | Trace what happens when a learner opens a document or browser | Outline only |
| 4 | Network fundamentals: PAN, LAN, WLAN, MAN, WAN | Classify a home, school, and mobile-device network | Outline only |
| 5 | Network devices and transmission media: NIC, switch, router, modem/ONT, access point, Ethernet, Wi-Fi | Label a simple home network diagram | Outline only |
| 6 | Addresses and protocols: MAC, IP, DNS, TCP/IP, ports (introductory) | Trace a browser request to a website | Drafted; needs review |
| 7 | Introduction to behaviorist AI: agents, environment, stimulus, response, feedback, rewards, and penalties | Identify the agent, environment, actions, and feedback in a simple game or navigation task | Outline only |
| 8 | How behaviorist AI learns: trial and error, positive and negative feedback, reward-based learning, and behavior adjustment | Use a simple scenario to show how an agent changes its actions after receiving rewards or penalties | Outline only |
| 9 | Basic applications and limitations of behaviorist AI | Compare a fixed rule-based game character with an agent that adjusts its behavior based on feedback; discuss why reward design matters | Outline only |
| 10 | Basic network safety and troubleshooting | Diagnose a fictional “website will not load” scenario using safe checks | Outline only |
| 11 | Review and assessment | Short quiz with answer explanations covering hardware, networks, website requests, and behaviorist AI | Outline only |

## Developed topic: How Data Travels from Your Computer to a Website
- **Core concepts:** DNS lookup, local network, router, internet path, server response, and browser rendering.
- **Worked example:** a learner enters a website name and follows the request/response sequence.
- **Visual:** a simple text diagram showing the main path.
- **Activity:** put stages in order and explain the purpose of DNS.
- **Expected outcome:** learner can describe the main stages without assuming that every network uses exactly the same physical path.
- **Status:** Drafted; needs peer review and source verification.

## Planned topic: Introduction to Behaviorist AI

### Core concepts
- **Agent:** the system that observes a situation and chooses an action.
- **Environment:** the surroundings or situation in which the agent operates.
- **Stimulus or observation:** information the agent receives about its current situation.
- **Action or response:** what the agent does in response to the situation.
- **Feedback:** information about the result of an action.
- **Reward and penalty:** signals that indicate whether an outcome is desirable or undesirable according to the system's objective.
- **Learning through interaction:** adjusting behavior based on experience and feedback.

### Explanation and example
Behaviorist AI can be introduced through the idea that an intelligent system adjusts its behavior based on interactions with its environment. For example, a virtual agent learning to navigate a maze may receive a positive reward for reaching the destination and a penalty for taking an undesirable action. Over repeated attempts, it can learn which actions are more likely to produce a favorable outcome.

A useful distinction is that a fixed rule-based system follows predefined instructions, whereas a learning agent can adjust its behavior based on experience. The two approaches can also be combined.

For a more technical introduction, the module can briefly explain **reinforcement learning**, a machine-learning approach in which an agent interacts with an environment and learns a policy that aims to maximize cumulative reward. This is a modern computational approach related to the broader idea of learning through consequences; not every behaviorist AI system necessarily uses reinforcement learning.

### Visual
A simple feedback-loop diagram:

**Environment → Observation → Agent chooses action → Environment changes → Feedback or reward → Agent adjusts behavior**

### Activity
Give learners a simple maze or game scenario and ask them to:
1. Identify the agent and its environment.
2. List the available actions.
3. Decide which outcomes should receive positive rewards or penalties.
4. Explain how feedback from repeated attempts could influence future actions.
5. Discuss what could happen if the reward system encourages the wrong behavior.

### Expected outcome
Learners can explain how an agent's behavior may change through feedback and experience, identify the components of a basic learning loop, and recognize that the reward system influences what the agent learns to do.

### Scope and limitations
- Keep the explanation conceptual and beginner-friendly.
- Avoid requiring advanced mathematics, neural-network implementation, or programming unless these are explicitly required by the teacher.
- Explain that reward-based learning does not guarantee human-like understanding or consistently correct behavior.
- Introduce the distinction between behaviorist ideas and modern reinforcement learning without treating them as identical.
- Discuss reward design as a potential limitation: an agent may optimize the specified reward without achieving the broader outcome its designer intended.

- **Status:** Outline only; substantive content, examples, and sources still need to be developed and reviewed.

## Scope and boundaries
**Included:** introductory hardware roles, network types, common network devices, wired/wireless links, basic addressing and DNS, a simplified website request, and introductory behaviorist AI concepts such as agents, feedback, rewards, penalties, and learning through interaction.

**Briefly introduced or deferred:** detailed CPU microarchitecture and electronic circuits; advanced subnetting and routing algorithms; enterprise network configuration; a full technical treatment of all OSI layers; advanced cryptography and cybersecurity; detailed reinforcement-learning algorithms, mathematical optimization, neural-network architectures, and advanced AI implementation. These topics may be added if the teacher expects them.

## Open questions for the teacher
1. Is binary/hexadecimal conversion required?
2. Must the full OSI model be taught, or is an introductory overview sufficient?
3. Are subnet masks/subnetting included in the assessment?
4. Is a practical hardware assembly or network configuration demonstration required?
5. Which network simulation tools, if any, are expected?
6. How much depth is required for behaviorist AI: a conceptual explanation, a demonstration of reinforcement learning, or a small practical implementation?
7. Is a specific AI tool, simulator, programming language, or learning environment required for the behaviorist AI activity?
8. Should the assessment distinguish classical behaviorist ideas from modern reinforcement learning?

## Review record
Do not mark this section `Checked` until a team member has reviewed the content. Record the actual reviewer, date, checks performed, findings, and corrections in the submission report.

The review should cover the accuracy of the hardware and networking explanations, the website-request sequence, the distinction between behaviorist concepts and reinforcement learning, the examples and activities, and the suitability of the content for beginner learners. Verify all technical claims against reliable sources and record any corrections made.
