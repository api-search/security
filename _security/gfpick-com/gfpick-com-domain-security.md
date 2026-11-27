---
api_specs:
- filename: gfpick-com-gcc-api-openapi.yml
  format: yaml
  label: GF Pick Gcc API
  slug: gfpick-com-gcc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gfpick-com/openapi/gfpick-com-gcc-api-openapi.yml
- filename: gfpick-com-saudi-api-openapi.yml
  format: yaml
  label: GF Pick Saudi API
  slug: gfpick-com-saudi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gfpick-com/openapi/gfpick-com-saudi-api-openapi.yml
- filename: gfpick-com-x402-api-openapi.yml
  format: yaml
  label: GF Pick X402 API
  slug: gfpick-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gfpick-com/openapi/gfpick-com-x402-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: gfpick.com
  spf: true
hosts:
- cert_expires: Dec 18 03:30:19 2026 GMT
  host: gfpick.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GF Pick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GF Pick, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: GF Pick
provider_slug: gfpick-com
slug: gfpick-com-domain-security
source_filename: gfpick-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gfpick.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 03:30:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gfpick.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gfpick-com/security/gfpick-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Shopping
- Global Sourcing
---
