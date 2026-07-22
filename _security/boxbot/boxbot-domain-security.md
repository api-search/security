---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: boxbot.io
  spf: true
hosts:
- cert_expires: Sep  6 04:28:16 2026 GMT
  host: www.boxbot.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boxbot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boxbot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Boxbot
provider_slug: boxbot
slug: boxbot-domain-security
source_filename: boxbot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boxbot.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 04:28:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: boxbot.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boxbot/refs/heads/main/security/boxbot-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Automation
- Supply Chain
- Robotics
- Warehouse Automation
- Logistics
- Artificial Intelligence
- Fulfillment
---
