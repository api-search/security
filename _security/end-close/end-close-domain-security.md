---
api_specs:
- filename: end-close-bank-account-balances-api-openapi.yml
  format: yaml
  label: End Close Bank Account Balances API
  slug: end-close-bank-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-close/refs/heads/main/openapi/end-close-bank-account-balances-api-openapi.yml
- filename: end-close-bank-accounts-api-openapi.yml
  format: yaml
  label: End Close Bank Accounts API
  slug: end-close-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-close/refs/heads/main/openapi/end-close-bank-accounts-api-openapi.yml
- filename: end-close-bulk-requests-api-openapi.yml
  format: yaml
  label: End Close Bulk Requests API
  slug: end-close-bulk-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-close/refs/heads/main/openapi/end-close-bulk-requests-api-openapi.yml
- filename: end-close-data-stream-property-definitions-api-openapi.yml
  format: yaml
  label: End Close Data Stream Property Definitions API
  slug: end-close-data-stream-property-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-close/refs/heads/main/openapi/end-close-data-stream-property-definitions-api-openapi.yml
- filename: end-close-data-streams-api-openapi.yml
  format: yaml
  label: End Close Data Streams API
  slug: end-close-data-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-close/refs/heads/main/openapi/end-close-data-streams-api-openapi.yml
- filename: end-close-import-batches-api-openapi.yml
  format: yaml
  label: End Close Import Batches API
  slug: end-close-import-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-close/refs/heads/main/openapi/end-close-import-batches-api-openapi.yml
- filename: end-close-reconciliation-exceptions-api-openapi.yml
  format: yaml
  label: End Close Reconciliation Exceptions API
  slug: end-close-reconciliation-exceptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-close/refs/heads/main/openapi/end-close-reconciliation-exceptions-api-openapi.yml
- filename: end-close-reconciliation-matches-api-openapi.yml
  format: yaml
  label: End Close Reconciliation Matches API
  slug: end-close-reconciliation-matches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-close/refs/heads/main/openapi/end-close-reconciliation-matches-api-openapi.yml
- filename: end-close-reconciliation-rules-api-openapi.yml
  format: yaml
  label: End Close Reconciliation Rules API
  slug: end-close-reconciliation-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-close/refs/heads/main/openapi/end-close-reconciliation-rules-api-openapi.yml
- filename: end-close-reconciliation-stories-api-openapi.yml
  format: yaml
  label: End Close Reconciliation Stories API
  slug: end-close-reconciliation-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-close/refs/heads/main/openapi/end-close-reconciliation-stories-api-openapi.yml
- filename: end-close-reconciliations-api-openapi.yml
  format: yaml
  label: End Close Reconciliations API
  slug: end-close-reconciliations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-close/refs/heads/main/openapi/end-close-reconciliations-api-openapi.yml
- filename: end-close-records-api-openapi.yml
  format: yaml
  label: End Close Records API
  slug: end-close-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-close/refs/heads/main/openapi/end-close-records-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: endclose.com
  spf: true
hosts:
- cert_expires: Sep 29 16:49:10 2026 GMT
  host: api.endclose.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: End Close Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for End Close, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: End Close
provider_slug: end-close
slug: end-close-domain-security
source_filename: end-close-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.endclose.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 16:49:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: endclose.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/end-close/refs/heads/main/security/end-close-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Reconciliation
- Payments
- Financial Operations
- Accounting
- Banking
- Data Integration
- Webhook
- Fintech
---
