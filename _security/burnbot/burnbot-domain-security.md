---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: burnbot.com
  spf: false
hosts:
- cert_expires: Aug 20 15:53:02 2026 GMT
  host: burnbot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Burnbot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Burnbot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Burnbot
provider_slug: burnbot
slug: burnbot-domain-security
source_filename: burnbot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: burnbot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 15:53:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: burnbot.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/burnbot/refs/heads/main/security/burnbot-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Wildfire Mitigation
- Fuels Management
- Robotics
- Autonomous Machines
- Climate
- Forestry
- Timber Operations
- Field Services
---
