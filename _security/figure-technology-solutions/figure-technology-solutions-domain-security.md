---
api_specs:
- filename: figure-technology-solutions-encryption-api-openapi.yml
  format: yaml
  label: Figure Technology Solutions Encryption API
  slug: figure-technology-solutions-encryption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-encryption-api-openapi.yml
- filename: figure-technology-solutions-heloc-application-requests-api-openapi.yml
  format: yaml
  label: Figure Technology Solutions HELOC application requests API
  slug: figure-technology-solutions-heloc-application-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-heloc-application-requests-api-openapi.yml
- filename: figure-technology-solutions-heloc-offers-api-openapi.yml
  format: yaml
  label: Figure Technology Solutions HELOC Offers API
  slug: figure-technology-solutions-heloc-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-heloc-offers-api-openapi.yml
- filename: figure-technology-solutions-loan-originator-requests-api-openapi.yml
  format: yaml
  label: Figure Technology Solutions Loan Originator requests API
  slug: figure-technology-solutions-loan-originator-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-loan-originator-requests-api-openapi.yml
- filename: figure-technology-solutions-loan-tape-v1-api-openapi.yml
  format: yaml
  label: Figure Technology Solutions Loan Tape V1 API
  slug: figure-technology-solutions-loan-tape-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-loan-tape-v1-api-openapi.yml
- filename: figure-technology-solutions-loan-tape-v2-api-openapi.yml
  format: yaml
  label: Figure Technology Solutions Loan Tape V2 API
  slug: figure-technology-solutions-loan-tape-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-loan-tape-v2-api-openapi.yml
- filename: figure-technology-solutions-payment-history-v1-api-openapi.yml
  format: yaml
  label: Figure Technology Solutions Payment History V1 API
  slug: figure-technology-solutions-payment-history-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-payment-history-v1-api-openapi.yml
- filename: figure-technology-solutions-payment-history-v2-api-openapi.yml
  format: yaml
  label: Figure Technology Solutions Payment History V2 API
  slug: figure-technology-solutions-payment-history-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-payment-history-v2-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figure.com
  spf: true
hosts:
- cert_expires: Sep 14 20:22:02 2026 GMT
  host: www.figure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 04:59:23 2026 GMT
  host: docs.figure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 04:59:23 2026 GMT
  host: api.figure.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Figure Technology Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Figure Technology Solutions, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Figure Technology Solutions
provider_slug: figure-technology-solutions
slug: figure-technology-solutions-domain-security
source_filename: figure-technology-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.figure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:22:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.figure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 04:59:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.figure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 04:59:23 2026 GMT\n  hsts: null\ndomains:\n- domain: figure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/security/figure-technology-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Lending
- HELOC
- Home Equity
- Mortgage
- Capital Markets
- Blockchain
- Loan Origination
- Financial-Services
---
