---
api_specs:
- filename: skyslope-forms-partnership-openapi.yml
  format: yaml
  label: SkySlope Partnership (Forms) API
  slug: skyslope-forms-partnership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyslope/refs/heads/main/openapi/skyslope-forms-partnership-openapi.yml
- filename: skyslope-offers-openapi.yml
  format: yaml
  label: SkySlope Offers API
  slug: skyslope-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyslope/refs/heads/main/openapi/skyslope-offers-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: skyslope.com
  spf: true
hosts:
- cert_expires: Oct  2 02:17:48 2026 GMT
  host: skyslope.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 02:17:48 2026 GMT
  host: forms.skyslope.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 02:17:48 2026 GMT
  host: offers.skyslope.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skyslope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SkySlope, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SkySlope
provider_slug: skyslope
slug: skyslope-domain-security
source_filename: skyslope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skyslope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:17:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: forms.skyslope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:17:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: offers.skyslope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:17:48 2026 GMT\n  hsts: false\ndomains:\n- domain: skyslope.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skyslope/refs/heads/main/security/skyslope-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Real Estate
- Transaction Management
- Digital Forms
- E-Signature
- Compliance
- PropTech
- Documents
---
