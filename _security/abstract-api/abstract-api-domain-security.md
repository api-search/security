---
api_specs:
- filename: abstract-api-vat-validation-api-openapi.yml
  format: yaml
  label: Abstract API VAT Validation API
  slug: abstract-api-vat-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-vat-validation-api-openapi.yml
- filename: abstract-api-abstract-avatars-api-api-openapi.yml
  format: yaml
  label: Abstract API Abstract Avatars API
  slug: abstract-api-abstract-avatars-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-abstract-avatars-api-api-openapi.yml
- filename: abstract-api-calculate-api-openapi.yml
  format: yaml
  label: Abstract API Calculate API
  slug: abstract-api-calculate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-calculate-api-openapi.yml
- filename: abstract-api-categories-api-openapi.yml
  format: yaml
  label: Abstract API Categories API
  slug: abstract-api-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-categories-api-openapi.yml
- filename: abstract-api-convert-api-openapi.yml
  format: yaml
  label: Abstract API Convert API
  slug: abstract-api-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-convert-api-openapi.yml
- filename: abstract-api-convert-time-api-openapi.yml
  format: yaml
  label: Abstract API Convert Time API
  slug: abstract-api-convert-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-convert-time-api-openapi.yml
- filename: abstract-api-current-time-api-openapi.yml
  format: yaml
  label: Abstract API Current Time API
  slug: abstract-api-current-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-current-time-api-openapi.yml
- filename: abstract-api-historical-api-openapi.yml
  format: yaml
  label: Abstract API Historical API
  slug: abstract-api-historical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-historical-api-openapi.yml
- filename: abstract-api-live-api-openapi.yml
  format: yaml
  label: Abstract API Live API
  slug: abstract-api-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-live-api-openapi.yml
- filename: abstract-api-upload-api-openapi.yml
  format: yaml
  label: Abstract API Upload API
  slug: abstract-api-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-upload-api-openapi.yml
- filename: abstract-api-url-api-openapi.yml
  format: yaml
  label: Abstract API URL API
  slug: abstract-api-url-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-url-api-openapi.yml
- filename: abstract-api-validate-api-openapi.yml
  format: yaml
  label: Abstract API Validate API
  slug: abstract-api-validate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-validate-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: abstractapi.com
  spf: false
hosts:
- cert_expires: Nov  8 10:22:22 2026 GMT
  host: www.abstractapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: app.abstractapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: emailreputation.abstractapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Abstract Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abstract API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Abstract API
provider_slug: abstract-api
slug: abstract-api-domain-security
source_filename: abstract-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abstractapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 10:22:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.abstractapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: emailreputation.abstractapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: abstractapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/security/abstract-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Avatars
- Company Enrichment
- Contacts
- Currency
- Email Validation
- Exchange Rates
- IBAN Validation
- Image Processing
- IP Geolocation
- IP Intelligence
- Phone Validation
- Public Holidays
- Screenshots
- Timezone
- VAT Validation
- Web Scraping
---
