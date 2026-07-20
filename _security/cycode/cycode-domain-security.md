---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@cycode.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cycode.com
  spf: true
hosts:
- cert_expires: Aug 19 07:55:36 2026 GMT
  host: cycode.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cycode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cycode, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cycode
provider_slug: cycode
slug: cycode-domain-security
source_filename: cycode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cycode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 07:55:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cycode.com\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@cycode.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cycode/refs/heads/main/security/cycode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Application Security
- Software Supply Chain Security
- ASPM
- DevSecOps
- Secrets Scanning
- SAST
- SCA
- Developer Tools
- MCP
- CLI
---
