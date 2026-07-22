---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nexiu.ai
  spf: true
hosts:
- cert_expires: Oct  2 12:34:39 2026 GMT
  host: nexiu.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nexiu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexiu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nexiu
provider_slug: nexiu
slug: nexiu-domain-security
source_filename: nexiu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexiu.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:34:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nexiu.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexiu/refs/heads/main/security/nexiu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Recruiting
- Human Resources
- Automation
- Artificial Intelligence
- WhatsApp
- Latin America
---
