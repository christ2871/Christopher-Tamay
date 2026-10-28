# DNS Amplification Analysis

## Results

Highest amplification:
## Results

Highest amplification:
1. amp-open.example.com - 55.6x
2. txt-bulk.example.org - 35.1x

Query type with largest response:
ANY

## Mitigations

1. Response Rate Limiting:
Limits how many DNS responses a server
can send, reducing amplification attacks.

2. BCP 38 Ingress Filtering:
Blocks packets with spoofed source IP
addresses, helping prevent DNS attacks.

## Reference

Trivedi, Cybersecurity: Theory,
Practice, and Ethics.
Denial-of-Service section.
