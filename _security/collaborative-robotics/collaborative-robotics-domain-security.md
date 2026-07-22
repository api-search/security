---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: co.bot
  spf: true
hosts:
- cert_expires: Oct  7 08:39:52 2026 GMT
  host: www.co.bot
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Collaborative Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Collaborative Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Collaborative Robotics
provider_slug: collaborative-robotics
slug: collaborative-robotics-domain-security
source_filename: collaborative-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.co.bot\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 08:39:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: co.bot\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/collaborative-robotics/refs/heads/main/security/collaborative-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Collaborative Robotics
- Physical AI
- Automation
- Artificial Intelligence
- Warehousing
- Manufacturing
- Healthcare
---
