---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: madebythomas.ai
  spf: false
hosts:
- cert_expires: Oct 16 19:51:29 2026 GMT
  host: madebythomas.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thomas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thomas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Thomas
provider_slug: thomas
slug: thomas-domain-security
source_filename: thomas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: madebythomas.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 19:51:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: madebythomas.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thomas/refs/heads/main/security/thomas-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- AI Agents
- Autonomous Agents
- B2B
- Y Combinator
- Startup
---
