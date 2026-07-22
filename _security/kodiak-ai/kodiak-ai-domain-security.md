---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kodiak.ai
  spf: true
hosts:
- cert_expires: Sep 19 22:52:15 2026 GMT
  host: kodiak.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kodiak Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kodiak AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kodiak AI
provider_slug: kodiak-ai
slug: kodiak-ai-domain-security
source_filename: kodiak-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kodiak.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:52:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kodiak.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kodiak-ai/refs/heads/main/security/kodiak-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Autonomous Vehicles
- Artificial Intelligence
- Robotics
- Trucking
- Freight
- Logistics
- Transportation
- Physical AI
- Defense
---
