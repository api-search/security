---
api_specs:
- filename: clearedpay-xyz-v1-openapi.json
  format: json
  label: Cleared Protocol API V1 API
  slug: cleared-protocol-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearedpay-xyz/openapi/_original/clearedpay-xyz-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clearedpay.xyz
  spf: false
hosts:
- cert_expires: Jan  8 01:22:33 2027 GMT
  host: clearedpay.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clearedpay Xyz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cleared, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Cleared
provider_slug: clearedpay-xyz
slug: clearedpay-xyz-domain-security
source_filename: clearedpay-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clearedpay.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 01:22:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clearedpay.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/clearedpay-xyz/security/clearedpay-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- USDC
- Invoicing
- Blockchain
- Contractor
---
