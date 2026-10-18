---
api_specs:
- filename: chrome-river-accounts-api-openapi.yml
  format: yaml
  label: Chrome River Accounts API
  slug: chrome-river-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-accounts-api-openapi.yml
- filename: chrome-river-allowances-api-openapi.yml
  format: yaml
  label: Chrome River Allowances API
  slug: chrome-river-allowances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-allowances-api-openapi.yml
- filename: chrome-river-cards-api-openapi.yml
  format: yaml
  label: Chrome River Cards API
  slug: chrome-river-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-cards-api-openapi.yml
- filename: chrome-river-categories-api-openapi.yml
  format: yaml
  label: Chrome River Categories API
  slug: chrome-river-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-categories-api-openapi.yml
- filename: chrome-river-company-api-openapi.yml
  format: yaml
  label: Chrome River Company API
  slug: chrome-river-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-company-api-openapi.yml
- filename: chrome-river-departments-api-openapi.yml
  format: yaml
  label: Chrome River Departments API
  slug: chrome-river-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-departments-api-openapi.yml
- filename: chrome-river-labels-api-openapi.yml
  format: yaml
  label: Chrome River Labels API
  slug: chrome-river-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-labels-api-openapi.yml
- filename: chrome-river-locations-api-openapi.yml
  format: yaml
  label: Chrome River Locations API
  slug: chrome-river-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-locations-api-openapi.yml
- filename: chrome-river-members-api-openapi.yml
  format: yaml
  label: Chrome River Members API
  slug: chrome-river-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-members-api-openapi.yml
- filename: chrome-river-merchant-categories-api-openapi.yml
  format: yaml
  label: Chrome River Merchant Categories API
  slug: chrome-river-merchant-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-merchant-categories-api-openapi.yml
- filename: chrome-river-oauth-api-openapi.yml
  format: yaml
  label: Chrome River OAuth API
  slug: chrome-river-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-oauth-api-openapi.yml
- filename: chrome-river-requisitions-api-openapi.yml
  format: yaml
  label: Chrome River Requisitions API
  slug: chrome-river-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-requisitions-api-openapi.yml
- filename: chrome-river-shared-links-api-openapi.yml
  format: yaml
  label: Chrome River Shared Links API
  slug: chrome-river-shared-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-shared-links-api-openapi.yml
- filename: chrome-river-shipping-addresses-api-openapi.yml
  format: yaml
  label: Chrome River Shipping Addresses API
  slug: chrome-river-shipping-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-shipping-addresses-api-openapi.yml
- filename: chrome-river-transactions-api-openapi.yml
  format: yaml
  label: Chrome River Transactions API
  slug: chrome-river-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/openapi/chrome-river-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: emburse.com
  spf: true
hosts:
- cert_expires: Nov 23 10:07:30 2026 GMT
  host: www.emburse.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chrome River Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chrome River, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chrome River
provider_slug: chrome-river
slug: chrome-river-domain-security
source_filename: chrome-river-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.emburse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 10:07:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: emburse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chrome-river/refs/heads/main/security/chrome-river-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Expense Management
- Software-as-a-Service
- Enterprise
- Travel
---
