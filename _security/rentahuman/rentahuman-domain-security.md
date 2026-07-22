---
api_specs:
- filename: rentahuman-openapi-original.yml
  format: yaml
  label: RentAHuman.ai API
  slug: rentahumanai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentahuman/refs/heads/main/openapi/rentahuman-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rentahuman.ai
  spf: true
hosts:
- cert_expires: Aug 28 17:43:19 2026 GMT
  host: rentahuman.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rentahuman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rentahuman, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rentahuman
provider_slug: rentahuman
slug: rentahuman-domain-security
source_filename: rentahuman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rentahuman.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 17:43:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rentahuman.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rentahuman/refs/heads/main/security/rentahuman-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplace
- AI Agents
- Human-in-the-Loop
- Gig Economy
- MCP
- Labor
- Payments
---
