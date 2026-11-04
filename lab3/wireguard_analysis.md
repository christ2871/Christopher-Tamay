# WireGuard Analysis

## Split Tunnel
AllowedIPs = 10.8.0.0/24, 192.168.50.0/24

Only traffic going to these two networks
will be routed through the VPN.
Other traffic uses the regular internet.

## Full Tunnel
AllowedIPs = 0.0.0.0/0

All IPv4 destinations are routed through
the VPN instead of just two networks.

## Privacy
A full tunnel protects more traffic
from observation on the local network.
However, the VPN provider can see
connection metadata.

## Availability
If the VPN connection fails, internet
access may be interrupted.

## Key Permissions
600 allows only the file owner to read
and write the private key.

644 would allow other users to read it,
which creates a security risk.
