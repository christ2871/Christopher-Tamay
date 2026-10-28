# Firewall ACL Test Results

## Accepted Connections

1. Internet to Web Server (HTTPS, port 443)
   Result: ALLOW

2. Web Server to Database (port 5432)
   Result: ALLOW

3. Admin Subnet to SSH (port 22)
   Result: ALLOW

## Denied Connections

4. Unauthorized SSH Access
   Result: DENY

5. Direct Internet Access to Database
   Result: DENY

6. Internet to Web Server (HTTP, port 80)
   Result: DENY
## Defense in Depth

Additional Rule:
iptables -I INPUT 1 -m conntrack --ctstate INVALID -j DROP

Explanation:
This rule blocks packets with invalid connection
states before they reach the other firewall rules.
It adds another layer of network protection.
