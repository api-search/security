---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cyera.com
  spf: true
hosts:
- cert_expires: Sep 12 06:13:32 2026 GMT
  host: www.cyera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cyera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cyera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cyera
provider_slug: cyera
slug: cyera-domain-security
source_filename: cyera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cyera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 06:13:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cyera.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cyera/refs/heads/main/security/cyera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Data Security
- DSPM
- Data Security Posture Management
- Data Classification
- Cloud Security
- Compliance
- MCP
- AI Security
---
