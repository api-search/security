---
api_specs:
- filename: fundmomentum-api-api-openapi.yml
  format: yaml
  label: Fund Momentum API
  slug: fundmomentum-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundmomentum/refs/heads/main/openapi/fundmomentum-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fundmomentum.vc
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: fundmomentum.vc
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fundmomentum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fund Momentum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fund Momentum
provider_slug: fundmomentum
slug: fundmomentum-domain-security
source_filename: fundmomentum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fundmomentum.vc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fundmomentum.vc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fundmomentum/refs/heads/main/security/fundmomentum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fundraising
- Venture-Capital
- Data-Intelligence
- AI-Agents
---
