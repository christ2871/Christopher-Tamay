# TLS Handshake Analysis

## Results
Protocol: TLS 1.3
Cipher: TLS_AES_256_GCM_SHA384
Certificate: lab.mac246.example.test

## Why This Cipher Is Secure

1. Forward Secrecy:
TLS 1.3 uses ephemeral key exchange.
Past sessions remain protected even if
a long-term private key is compromised.

2. Authenticated Encryption:
AES-GCM provides confidentiality and
integrity, protecting data from being
read or modified without detection.

3. Key Strength:
AES-256 uses a 256-bit encryption key,
providing strong protection.

## TLS vs WireGuard

TLS:
Protects application connections,
such as HTTPS websites.

WireGuard:
Protects IP traffic through an
encrypted VPN tunnel.

Both provide confidentiality and
integrity.

WireGuard uses AllowedIPs to determine
which IP addresses use the VPN.
TLS does not have an equivalent setting.

## Reference
Trivedi, Cybersecurity: Theory,
Practice, and Ethics, Chapter 2.
