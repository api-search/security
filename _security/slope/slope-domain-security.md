---
api_specs:
- filename: slope-auth-api-openapi.yml
  format: yaml
  label: Slope Auth API
  slug: slope-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slope/refs/heads/main/openapi/slope-auth-api-openapi.yml
- filename: slope-customers-api-openapi.yml
  format: yaml
  label: Slope Customers API
  slug: slope-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slope/refs/heads/main/openapi/slope-customers-api-openapi.yml
- filename: slope-files-api-openapi.yml
  format: yaml
  label: Slope Files API
  slug: slope-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slope/refs/heads/main/openapi/slope-files-api-openapi.yml
- filename: slope-orders-api-openapi.yml
  format: yaml
  label: Slope Orders API
  slug: slope-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slope/refs/heads/main/openapi/slope-orders-api-openapi.yml
- filename: slope-payout-accounts-api-openapi.yml
  format: yaml
  label: Slope Payout Accounts API
  slug: slope-payout-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slope/refs/heads/main/openapi/slope-payout-accounts-api-openapi.yml
- filename: slope-persons-api-openapi.yml
  format: yaml
  label: Slope Persons API
  slug: slope-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slope/refs/heads/main/openapi/slope-persons-api-openapi.yml
- filename: slope-prescreens-api-openapi.yml
  format: yaml
  label: Slope Prescreens API
  slug: slope-prescreens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slope/refs/heads/main/openapi/slope-prescreens-api-openapi.yml
- filename: slope-simulation-api-openapi.yml
  format: yaml
  label: Slope Simulation API
  slug: slope-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slope/refs/heads/main/openapi/slope-simulation-api-openapi.yml
- filename: slope-transactions-api-openapi.yml
  format: yaml
  label: Slope Transactions API
  slug: slope-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slope/refs/heads/main/openapi/slope-transactions-api-openapi.yml
- filename: slope-user-links-api-openapi.yml
  format: yaml
  label: Slope User Links API
  slug: slope-user-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slope/refs/heads/main/openapi/slope-user-links-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: slopepay.com
  spf: true
hosts:
- cert_expires: Oct  1 12:58:48 2026 GMT
  host: www.slopepay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: api.slopepay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: api.sandbox.slopepay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Slope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Slope, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Slope
provider_slug: slope
slug: slope-domain-security
source_filename: slope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.slopepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 12:58:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.slopepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: null\n- host: api.sandbox.slopepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: slopepay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slope/refs/heads/main/security/slope-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Embedded Finance
- BNPL
- Lending
- Credit
- B2B
- Checkout
---
