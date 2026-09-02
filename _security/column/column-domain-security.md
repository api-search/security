---
api_specs:
- filename: column-ach-transfers-api-openapi.yml
  format: yaml
  label: Column ACH Transfers API
  slug: column-ach-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-ach-transfers-api-openapi.yml
- filename: column-wire-transfers-api-openapi.yml
  format: yaml
  label: Column Wire Transfers API
  slug: column-wire-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-wire-transfers-api-openapi.yml
- filename: column-international-wires-api-openapi.yml
  format: yaml
  label: Column International Wires API
  slug: column-international-wires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-international-wires-api-openapi.yml
- filename: column-realtime-transfers-api-openapi.yml
  format: yaml
  label: Column Realtime Transfers API
  slug: column-realtime-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-realtime-transfers-api-openapi.yml
- filename: column-book-transfers-api-openapi.yml
  format: yaml
  label: Column Book Transfers API
  slug: column-book-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-book-transfers-api-openapi.yml
- filename: column-asyncapi.yml
  format: yaml
  label: Column Webhooks
  slug: column-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-asyncapi.yml
- filename: column-account-numbers-api-openapi.yml
  format: yaml
  label: Column Account Numbers API
  slug: column-account-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-account-numbers-api-openapi.yml
- filename: column-ach-transfers-api-openapi.yml
  format: yaml
  label: Column ACH Transfers API
  slug: column-ach-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-ach-transfers-api-openapi.yml
- filename: column-bank-accounts-api-openapi.yml
  format: yaml
  label: Column Bank Accounts API
  slug: column-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-bank-accounts-api-openapi.yml
- filename: column-book-transfers-api-openapi.yml
  format: yaml
  label: Column Book Transfers API
  slug: column-book-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-book-transfers-api-openapi.yml
- filename: column-check-transfers-api-openapi.yml
  format: yaml
  label: Column Check Transfers API
  slug: column-check-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-check-transfers-api-openapi.yml
- filename: column-counterparties-api-openapi.yml
  format: yaml
  label: Column Counterparties API
  slug: column-counterparties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-counterparties-api-openapi.yml
- filename: column-entities-api-openapi.yml
  format: yaml
  label: Column Entities API
  slug: column-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-entities-api-openapi.yml
- filename: column-events-api-openapi.yml
  format: yaml
  label: Column Events API
  slug: column-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-events-api-openapi.yml
- filename: column-international-wires-api-openapi.yml
  format: yaml
  label: Column International Wires API
  slug: column-international-wires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-international-wires-api-openapi.yml
- filename: column-realtime-transfers-api-openapi.yml
  format: yaml
  label: Column Realtime Transfers API
  slug: column-realtime-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-realtime-transfers-api-openapi.yml
- filename: column-webhooks-api-openapi.yml
  format: yaml
  label: Column Webhooks API
  slug: column-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-webhooks-api-openapi.yml
- filename: column-wire-transfers-api-openapi.yml
  format: yaml
  label: Column Wire Transfers API
  slug: column-wire-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-wire-transfers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: column.com
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: column.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.column.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: docs.column.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Column Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Column, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Column
provider_slug: column
slug: column-domain-security
source_filename: column-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: column.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: false\n- host: api.column.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\n- host: docs.column.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: column.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/security/column-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fintech
- Banking
- Backend-as-a-Service
- ACH
- Wires
---
