---
api_specs:
- filename: sbc-openapi-generated.yml
  format: yaml
  label: SBC API
  slug: sbc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sbc/openapi/_ae-authored/sbc-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stablecoin.xyz
  spf: true
hosts:
- cert_expires: Jan  7 16:24:14 2027 GMT
  host: stablecoin.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sbc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SBC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SBC
provider_slug: sbc
slug: sbc-domain-security
source_filename: sbc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stablecoin.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 16:24:14 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stablecoin.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/sbc/security/sbc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- FinTech
- Payments
- Stablecoin
- API
---
