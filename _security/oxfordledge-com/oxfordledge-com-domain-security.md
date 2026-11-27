---
api_specs:
- filename: oxfordledge-com-api-openapi.yml
  format: yaml
  label: Oxford Ledge API API
  slug: oxford-ledge-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oxfordledge-com/openapi/_original/oxfordledge-com-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oxfordledge.com
  spf: true
hosts:
- cert_expires: Dec 23 07:20:03 2026 GMT
  host: oxfordledge.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oxford Ledge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oxford Ledge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Oxford Ledge
provider_slug: oxfordledge-com
slug: oxfordledge-com-domain-security
source_filename: oxfordledge-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oxfordledge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 07:20:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oxfordledge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/oxfordledge-com/security/oxfordledge-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Research
- Market Data
- SEC Filings
- Investor
- Students
---
