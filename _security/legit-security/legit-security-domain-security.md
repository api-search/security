---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: legitsecurity.com
  spf: true
hosts:
- cert_expires: Aug 21 18:59:55 2026 GMT
  host: www.legitsecurity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Legit Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Legit Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Legit Security
provider_slug: legit-security
slug: legit-security-domain-security
source_filename: legit-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.legitsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 18:59:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: legitsecurity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/legit-security/refs/heads/main/security/legit-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Application Security
- ASPM
- DevSecOps
- Software Supply Chain Security
- Secrets Detection
- SAST
- SCA
- Compliance
- AI Security
- MCP
---
