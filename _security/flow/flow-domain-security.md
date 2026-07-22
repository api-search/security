---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flowengineering.com
  spf: true
hosts:
- cert_expires: Aug 25 20:52:35 2026 GMT
  host: flowengineering.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Flow
provider_slug: flow
slug: flow-domain-security
source_filename: flow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flowengineering.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 20:52:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: flowengineering.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flow/refs/heads/main/security/flow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Requirements Management
- Systems Engineering
- Hardware Engineering
- Product Lifecycle Management
- Engineering
- Compliance
- AI Agents
---
