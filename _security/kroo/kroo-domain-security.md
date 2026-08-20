---
api_specs:
- filename: obie-account-info-openapi.yaml
  format: yaml
  label: Kroo Account and Transaction Information API
  slug: kroo-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kroo/refs/heads/main/openapi/obie-account-info-openapi.yaml
- filename: obie-payment-initiation-openapi.yaml
  format: yaml
  label: Kroo Payment Initiation API
  slug: kroo-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kroo/refs/heads/main/openapi/obie-payment-initiation-openapi.yaml
- filename: obie-confirmation-funds-openapi.yaml
  format: yaml
  label: Kroo Confirmation of Funds API
  slug: kroo-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kroo/refs/heads/main/openapi/obie-confirmation-funds-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kroo.com
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: banfico.io
  spf: true
hosts:
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: www.kroo.com
  hsts: true
  hsts_max_age: 31104000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: developer.kroo.banfico.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kroo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kroo, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Kroo
provider_slug: kroo
slug: kroo-domain-security
source_filename: kroo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kroo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31104000\n- host: developer.kroo.banfico.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: kroo.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: banfico.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kroo/refs/heads/main/security/kroo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
- Challenger Bank
- Fintech
---
