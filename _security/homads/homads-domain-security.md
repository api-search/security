---
api_specs:
- filename: homads-openapi.yml
  format: yaml
  label: Homads Rental Market Data
  slug: rental-market-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/homads/refs/heads/main/openapi/homads-openapi.yml
- filename: homads-openapi.yml
  format: yaml
  label: Homads Rent Comparison
  slug: rent-comparison
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/homads/refs/heads/main/openapi/homads-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: homads.com
  spf: true
hosts:
- cert_expires: Sep  5 18:19:56 2026 GMT
  host: homads.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Homads Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Homads, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Homads
provider_slug: homads
slug: homads-domain-security
source_filename: homads-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: homads.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 18:19:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: homads.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/homads/refs/heads/main/security/homads-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Rental
- Mid-Term Rental
- Real Estate
- Marketplace
- Neighborhood Data
---
