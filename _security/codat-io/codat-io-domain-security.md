---
api_specs:
- filename: codat-io-accounting-api-openapi.yml
  format: yaml
  label: Codat Accounting API
  slug: codat-io-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-accounting-api-openapi.yml
- filename: codat-io-bank-feeds-api-openapi.yml
  format: yaml
  label: Codat Bank Feeds API
  slug: codat-io-bank-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-bank-feeds-api-openapi.yml
- filename: codat-io-banking-api-openapi.yml
  format: yaml
  label: Codat Banking API
  slug: codat-io-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-banking-api-openapi.yml
- filename: codat-io-commerce-api-openapi.yml
  format: yaml
  label: Codat Commerce API
  slug: codat-io-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-commerce-api-openapi.yml
- filename: codat-io-companies-api-openapi.yml
  format: yaml
  label: Codat Companies API
  slug: codat-io-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-companies-api-openapi.yml
- filename: codat-io-connections-api-openapi.yml
  format: yaml
  label: Codat Connections API
  slug: codat-io-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-connections-api-openapi.yml
- filename: codat-io-expenses-api-openapi.yml
  format: yaml
  label: Codat Expenses API
  slug: codat-io-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-expenses-api-openapi.yml
- filename: codat-io-integrations-api-openapi.yml
  format: yaml
  label: Codat Integrations API
  slug: codat-io-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-integrations-api-openapi.yml
- filename: codat-io-lending-api-openapi.yml
  format: yaml
  label: Codat Lending API
  slug: codat-io-lending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-lending-api-openapi.yml
- filename: codat-io-manage-data-api-openapi.yml
  format: yaml
  label: Codat Manage data API
  slug: codat-io-manage-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-manage-data-api-openapi.yml
- filename: codat-io-payables-api-openapi.yml
  format: yaml
  label: Codat Payables API
  slug: codat-io-payables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-payables-api-openapi.yml
- filename: codat-io-sync-for-commerce-api-openapi.yml
  format: yaml
  label: Codat Sync for Commerce API
  slug: codat-io-sync-for-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-sync-for-commerce-api-openapi.yml
- filename: codat-io-webhooks-api-openapi.yml
  format: yaml
  label: Codat Webhooks API
  slug: codat-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: codat.io
  spf: true
hosts:
- cert_expires: Sep 14 03:39:22 2026 GMT
  host: www.codat.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 19:25:16 2026 GMT
  host: docs.codat.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 11:57:27 2026 GMT
  host: api.codat.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codat Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codat, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Codat
provider_slug: codat-io
slug: codat-io-domain-security
source_filename: codat-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.codat.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:39:22 2026 GMT\n  hsts: false\n- host: docs.codat.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 19:25:16 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.codat.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 11:57:27 2026 GMT\n  hsts: null\ndomains:\n- domain: codat.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/security/codat-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Business Data
- Accounting
- Banking
- Commerce
- Fintech
- Lending
- Financial Data
---
