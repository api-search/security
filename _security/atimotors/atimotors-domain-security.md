---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atirobotics.ai
  spf: true
hosts:
- cert_expires: Nov 18 08:03:47 2026 GMT
  host: www.atirobotics.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atimotors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atimotors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Atimotors
provider_slug: atimotors
slug: atimotors-domain-security
source_filename: atimotors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atirobotics.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 08:03:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atirobotics.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atimotors/refs/heads/main/security/atimotors-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Robotics
- Material Handling
- Industrial Automation
- AI
- Factory Software
- Robots-as-a-Service
---
