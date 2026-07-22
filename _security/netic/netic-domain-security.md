---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: netic.ai
  spf: true
hosts:
- cert_expires: Aug 21 13:40:27 2026 GMT
  host: www.netic.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Netic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Netic
provider_slug: netic
slug: netic-domain-security
source_filename: netic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.netic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 13:40:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: netic.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netic/refs/heads/main/security/netic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Artificial Intelligence
- Autonomous Agents
- Home Services
- Field Service
- Voice AI
- Automation
- SaaS
---
