---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: claroty.com
  spf: true
hosts:
- cert_expires: Aug 13 23:18:21 2026 GMT
  host: www.claroty.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Claroty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Claroty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Claroty
provider_slug: claroty
slug: claroty-domain-security
source_filename: claroty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.claroty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 23:18:21 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: claroty.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/security/claroty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- OT Security
- Cyber-Physical Systems
- IoT Security
- Industrial Control Systems
- Threat Detection
- Exposure Management
- Healthcare Security
---
