---
api_specs:
- filename: obie-opendata-swagger.json
  format: json
  label: Coventry Building Society Open Data FCA Service Metrics API
  slug: coventry-building-society-open-data-fca-service-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coventry-building-society/refs/heads/main/openapi/obie-opendata-swagger.json
- filename: obie-account-info-openapi.yaml
  format: yaml
  label: Coventry Building Society Account & Transaction Information API (AIS)
  slug: coventry-building-society-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coventry-building-society/refs/heads/main/openapi/obie-account-info-openapi.yaml
- filename: obie-payment-initiation-openapi.yaml
  format: yaml
  label: Coventry Building Society Payment Initiation API (PIS)
  slug: coventry-building-society-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coventry-building-society/refs/heads/main/openapi/obie-payment-initiation-openapi.yaml
- filename: obie-confirmation-funds-openapi.yaml
  format: yaml
  label: Coventry Building Society Confirmation of Funds API (CBPII)
  slug: coventry-building-society-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coventry-building-society/refs/heads/main/openapi/obie-confirmation-funds-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coventrybuildingsociety.co.uk
  spf: true
hosts:
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: www.coventrybuildingsociety.co.uk
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: developer.coventrybuildingsociety.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: connect.coventrybuildingsociety.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Coventry Building Society Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coventry Building Society, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Coventry Building Society
provider_slug: coventry-building-society
slug: coventry-building-society-domain-security
source_filename: coventry-building-society-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coventrybuildingsociety.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: developer.coventrybuildingsociety.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: connect.coventrybuildingsociety.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: coventrybuildingsociety.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coventry-building-society/refs/heads/main/security/coventry-building-society-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Financial Services
- Banking
- Building Society
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Confirmation of Funds
- Fintech
---
