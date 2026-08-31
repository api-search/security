---
api_specs:
- filename: bybe-clips-api-openapi.yml
  format: yaml
  label: BYBE Clips API
  slug: bybe-clips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bybe/refs/heads/main/openapi/bybe-clips-api-openapi.yml
- filename: bybe-consumers-api-openapi.yml
  format: yaml
  label: BYBE Consumers API
  slug: bybe-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bybe/refs/heads/main/openapi/bybe-consumers-api-openapi.yml
- filename: bybe-manufacturers-api-openapi.yml
  format: yaml
  label: BYBE Manufacturers API
  slug: bybe-manufacturers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bybe/refs/heads/main/openapi/bybe-manufacturers-api-openapi.yml
- filename: bybe-offers-api-openapi.yml
  format: yaml
  label: BYBE Offers API
  slug: bybe-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bybe/refs/heads/main/openapi/bybe-offers-api-openapi.yml
- filename: bybe-products-api-openapi.yml
  format: yaml
  label: BYBE Products API
  slug: bybe-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bybe/refs/heads/main/openapi/bybe-products-api-openapi.yml
- filename: bybe-redemptions-api-openapi.yml
  format: yaml
  label: BYBE Redemptions API
  slug: bybe-redemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bybe/refs/heads/main/openapi/bybe-redemptions-api-openapi.yml
- filename: bybe-stores-api-openapi.yml
  format: yaml
  label: BYBE Stores API
  slug: bybe-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bybe/refs/heads/main/openapi/bybe-stores-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bybe.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bybe.io
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: bybe.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: docs.bybe.io
  hsts: true
  hsts_evidence: 'docs.bybe.io redirects to https://api.bybe.io/docs/index.html, which returns HTTP 200 with strict-transport-security: max-age=31536000; includeSubDomains (observed 2026-08-13).'
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: api.bybe.io
  hsts: true
  hsts_evidence: 'strict-transport-security: max-age=31536000; includeSubDomains observed on all three of GET / (404), GET /v1/offers (401) and GET /docs/index.html (200), 2026-08-13. The mechanical probe recorded null here because the host root answers 404; corrected from the direct observation above.'
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bybe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BYBE, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BYBE
provider_slug: bybe
slug: bybe-domain-security
source_filename: bybe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bybe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: false\n- host: docs.bybe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_evidence: >-\n    docs.bybe.io redirects to https://api.bybe.io/docs/index.html, which returns HTTP 200 with\n    strict-transport-security: max-age=31536000; includeSubDomains (observed 2026-08-13).\n- host: api.bybe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_evidence: >-\n    strict-transport-security: max-age=31536000; includeSubDomains observed on all three of\n    GET / (404), GET /v1/offers (401) and GET /docs/index.html (200), 2026-08-13. The mechanical\n\
  \    probe recorded null here because the host root answers 404; corrected from the direct\n    observation above.\ndomains:\n- domain: bybe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: bybe.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bybe/refs/heads/main/security/bybe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Alcohol
- Beverages
- Promotions
- Rebates
- Marketing
- Retail
- CPG
- Loyalty
- Payments
- Disbursements
- Compliance
---
