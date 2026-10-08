# Sanitized Scan Summary

- Target: lab.local (192.168.x.x - sanitized)
- Ports: 80/http, 22/ssh
- Service: Apache/2.4.x
- Finding 1: CVE-2007-6750 validated - Server vulnerable to Slowloris (connection exhaustion)
- Finding 2: Missing HSTS, CSP, X-Frame-Options
- Finding 3: No rate limiting

Mitigation: Implement mod_reqtimeout, Nginx reverse proxy, fail2ban.
