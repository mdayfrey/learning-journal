# Day 2

## CS50 Week 0: Key Concepts

**Computer Science**

- Computer science = problem solving
    - Take input → produce correct output (problem solving)
- **Goal**: learn how to think, not just code
- Not just representing data but processing it
- Use logical, structured thinking (computational thinking)
- Everything builds in layers (abstraction): bits → data → algorithms → programs → software → AI
- AI makes building software faster (debugging, generating features), but fundamentals are still required as humans remain the decision-makers

**Data Representation**

- Computers understand binary
- **They use transistors that switch on/off → represent 0 and 1**
- **Core chain**: transistors -> bits -> bytes -> data
- **Bit** (binary digit) = smallest unit
- **Byte** = 8 bits
- Same binary data can represent different things depending on context

**Different Data Types**

- **Numbers** = stored as binary
- **Text/characters**
    - ASCII -> maps characters to numbers (e.g., A = 65)
    - Unicode -> supports all languages + emojis
- **Images**
    - Made of pixels
    - Each pixel = RGB values (0–255)
- **Video** = sequence of images (frames)
- **Sound** = frequency (pitch), amplitude (loudness) + duration

**Programming Basics**

- **Algorithm**
    - **Step-by-step instructions to solve a problem**
    - Idea before code
    - Input → Algorithm → Output
    - Quality matters:
        - Must be correct + efficient
        - Linear search → one-by-one (slow)
        - Binary search → divide in half each step (much faster)
        - Better design = fewer steps/less time
- **Pseudocode**
    - Human-readable version of an algorithm
    - Used to plan before coding
- **Code = implementation of an algorithm**
- **Core Constructs**
    - Functions → reusable actions
        - Side effect → visible output
        - Return value → internal output
    - Variables → store data
    - Conditionals → decisions (if/else)
    - Loops → repetition
    - Booleans -> True/False values (used in conditionals)
- **Programming Principles**
    - Good code is correct, efficient, clean + reusable
    - Avoid repetition → use functions
    - Don’t copy + paste -> use loops
    - Break problems into smaller parts

**Tools: Scratch**

- Teaches core logic without syntax
- Same concepts as real languages

## What Happens When You Type a URL

1. **You press the key** — your keyboard sends an electrical signal to your operating system
2. **Browser parses the URL** — it figures out the protocol (https), the domain (google.com), and the path (/)
3. **DNS lookup** — your computer asks "what's the IP address for google.com?" and gets back something like `142.250.80.46`
4. **TCP connection** — your computer opens a reliable connection to that IP address (like dialing a phone number and waiting for someone to pick up)
5. **TLS/SSL handshake** — your browser and the server agree on encryption so nobody can eavesdrop (the "s" in https)
6. **HTTP request** — your browser sends a message: "GET me the homepage please"
7. **Server processes it** — the request might hit a load balancer, then a web server, then an application server, then a database
8. **HTTP response** — the server sends back HTML, CSS, and JavaScript
9. **Browser renders the page** — it turns that code into the visual page you see