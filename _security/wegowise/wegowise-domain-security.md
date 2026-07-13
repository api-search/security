---
api_specs:
- filename: wegowise-openapi.yml
  format: yaml
  label: WegoWise API
  slug: wegowise
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wegowise/refs/heads/main/openapi/wegowise-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wegowise.com
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.wegowise.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Wegowise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WegoWise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: WegoWise
provider_slug: wegowise
slug: wegowise-domain-security
source_filename: wegowise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wegowise.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: wegowise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wegowise/refs/heads/main/security/wegowise-domain-security.yml
summary_line: TLSv1.2
tags:
- Benchmarking
- Building Energy
- Energy Efficiency
- Multifamily
- Property Management
- Utility Data
---
