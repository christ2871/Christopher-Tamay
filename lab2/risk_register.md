| Asset | Threat | Likelihood | Impact | Inherent Risk | Treatment | Control | Residual Risk |
|---|---|---|---|---|---|---|---|

Linux VM | Unauthorized access | M | M | M | Mitigate | Strong passwords + MFA | L 
Windows analysis host | Malware infection | H | H | H | Mitigate | Antivirus/endpoint protection + regular updates | M
Linux VM #2 | Unpatched software vulnerability | M | M | M | Mitigate | Regular security updates and patching | M
Linux VM #3 | Misconfigured firewall | M | M | M | Mitigate | Review firewall rules and block unnecessary ports/services | L

The Linux VM had a Medium inherent risk of unauthorized access. After implementing strong passwords 
and multi-factor authentication,
 the residual risk was reduced to Low because these controls make unauthorized login more difficult.
