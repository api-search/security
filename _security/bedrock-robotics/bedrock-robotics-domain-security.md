---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bedrockrobotics.com
  spf: true
hosts:
- cert_expires: Oct  9 00:18:53 2026 GMT
  host: bedrockrobotics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bedrock Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bedrock Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bedrock Robotics
provider_slug: bedrock-robotics
slug: bedrock-robotics-domain-security
source_filename: bedrock-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bedrockrobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 00:18:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bedrockrobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bedrock-robotics/refs/heads/main/security/bedrock-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Autonomy
- Construction
- Heavy Equipment
- Autonomous Machinery
- Artificial Intelligence
- Physical AI
---
