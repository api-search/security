---
api_specs:
- filename: fis-accounts-api-openapi.yml
  format: yaml
  label: FIS Global Accounts API
  slug: fis-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-accounts-api-openapi.yml
- filename: fis-ach-api-openapi.yml
  format: yaml
  label: FIS Global ACH API
  slug: fis-ach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-ach-api-openapi.yml
- filename: fis-payments-api-openapi.yml
  format: yaml
  label: FIS Global Payments API
  slug: fis-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-payments-api-openapi.yml
- filename: fis-transactions-api-openapi.yml
  format: yaml
  label: FIS Global Transactions API
  slug: fis-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-transactions-api-openapi.yml
- filename: fis-wire-transfers-api-openapi.yml
  format: yaml
  label: FIS Global Wire Transfers API
  slug: fis-wire-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-wire-transfers-api-openapi.yml
- filename: fis-accounting-data-as-a-service-openapi.json
  format: json
  label: FIS Accounting Data as a Service
  slug: fis-accounting-data-as-a-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/_original/fis-accounting-data-as-a-service-openapi.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "visa.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fisglobal.com
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.fisglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: codeconnect.fisglobal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.fisglobal.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Fis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FIS Global, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FIS Global
provider_slug: fis
slug: fis-domain-security
source_filename: fis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fisglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: null\n- host: codeconnect.fisglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fisglobal.com\n  https: false\ndomains:\n- domain: fisglobal.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"visa.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/security/fis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Core Banking
- Financial-Services
- Payments
- Fintech
---
