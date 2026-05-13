*This project has been created as part of the 42 curriculum by jjorda.*

## Description

NetPractice is a practical networking exercise in which you configure 10 small-scale simulated networks directly in your browser. The goal is to fix broken network diagrams by correctly assigning IP addresses, subnet masks, routes, and gateways so that all hosts can communicate as required.

## Instructions

**Running the training interface:**

1. Download and extract the project archive.
2. Run `./run.sh` from the extracted folder — this starts a local web server and opens the interface in your browser.
3. If `run.sh` fails: `python3 -m http.server 49242`, then navigate to `http://localhost:49242`.

**Important:** Enter your 42 login in the interface before starting — Moulinette uses it to generate your personal configuration.

**Completing levels:**

- Modify the unshaded fields in each network diagram until the configuration is valid.
- Click **Check again** to verify.
- Click **Get my config** to export the level's configuration file before proceeding.

## Resources

**Concepts studied:**

- TCP/IP addressing (IPv4)
- Subnet masks and CIDR notation — e.g. `/28` gives a mask of `255.255.255.240`, leaving 4 bits for hosts: 16 addresses per subnet, of which 14 are usable (network address and broadcast are reserved)
- Default gateways and routing tables
- Routers and switches
- OSI model layers (focus on Network layer / Layer 3)

**References:**

- [RFC 791 – Internet Protocol](https://datatracker.ietf.org/doc/html/rfc791)
- [Subnetting Practice](https://subnettingpractice.com/)
- [Cisco – IP Addressing and Subnetting](https://www.cisco.com/c/en/us/support/docs/ip/routing-information-protocol-rip/13788-3.html)

**AI usage:**

Claude (Anthropic) was used to:
- Help to write this README.
- Help understand the theory behind networking concepts (subnetting, routing, gateways, etc.).
- Help solve the exercises by explaining errors and guiding through configurations.