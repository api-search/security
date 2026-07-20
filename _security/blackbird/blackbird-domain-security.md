---
api_specs:
- filename: blackbird-flynet-openapi-original.yml
  format: yaml
  label: Flynet API
  slug: flynet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-flynet-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blackbird.xyz
  spf: true
hosts:
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: blackbird.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: api.staging.blackbird.xyz
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Blackbird Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blackbird, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Blackbird
provider_slug: blackbird
slug: blackbird-domain-security
source_filename: blackbird-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blackbird.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: false\n- host: api.staging.blackbird.xyz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: blackbird.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/security/blackbird-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Restaurants
- Loyalty
- Payments
- Dining
- Membership
- Crypto
- Blockchain
- Web3
---
