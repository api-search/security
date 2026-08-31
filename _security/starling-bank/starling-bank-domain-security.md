---
api_specs:
- filename: starling-bank-atm-api-openapi.yml
  format: yaml
  label: Starling Bank ATM API
  slug: starling-bank-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starling-bank/refs/heads/main/openapi/starling-bank-atm-api-openapi.yml
- filename: starling-bank-bca-api-openapi.yml
  format: yaml
  label: Starling Bank BCA API
  slug: starling-bank-bca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starling-bank/refs/heads/main/openapi/starling-bank-bca-api-openapi.yml
- filename: starling-bank-branch-api-openapi.yml
  format: yaml
  label: Starling Bank Branch API
  slug: starling-bank-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starling-bank/refs/heads/main/openapi/starling-bank-branch-api-openapi.yml
- filename: starling-bank-ccc-api-openapi.yml
  format: yaml
  label: Starling Bank CCC API
  slug: starling-bank-ccc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starling-bank/refs/heads/main/openapi/starling-bank-ccc-api-openapi.yml
- filename: starling-bank-pca-api-openapi.yml
  format: yaml
  label: Starling Bank PCA API
  slug: starling-bank-pca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starling-bank/refs/heads/main/openapi/starling-bank-pca-api-openapi.yml
- filename: starling-bank-sme-api-openapi.yml
  format: yaml
  label: Starling Bank SME API
  slug: starling-bank-sme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starling-bank/refs/heads/main/openapi/starling-bank-sme-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: starlingbank.com
  spf: true
hosts:
- cert_expires: Dec 27 12:06:52 2026 GMT
  host: www.starlingbank.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 12:06:52 2026 GMT
  host: developer.starlingbank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 12:06:52 2026 GMT
  host: api.starlingbank.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Starling Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Starling Bank, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Starling Bank
provider_slug: starling-bank
slug: starling-bank-domain-security
source_filename: starling-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.starlingbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 12:06:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.starlingbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 12:06:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.starlingbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 12:06:52 2026 GMT\n  hsts: null\ndomains:\n- domain: starlingbank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starling-bank/refs/heads/main/security/starling-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Challenger Bank
- Fintech
- FAPI
---
