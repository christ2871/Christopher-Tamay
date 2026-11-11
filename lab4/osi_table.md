| Layer | Indicator | Evidence source | Interpretation |
|---|---|---|---|
| L2 (MAC) ARP request/reply for 10.12.0.1 | capture.pcap, frames 8-9 | Host discovers router MAC address|
| L3 (IP) 198.51.100.23 contacts 10.12.0.15 | capture.pcap, IP conversations | External IP communications with campus Host |
| L4 (TCP or UDP) |TCP SYN attempts to port 22 and 80 |capture.pcap, frames 10,26,35|Connection attemps to SSH and HTTP |
| L5 to L6 (session, presentation) TLS packets | capture.pcap, frames 47-50 | Encrypted session traffic observed |
| L7 (application) Failed SSH logins and suspicious HTTP requests | auth.log; http_access.log | Possible password guessing and command execution attempt |
