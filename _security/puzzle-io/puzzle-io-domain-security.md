---
api_specs:
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Companies API
  slug: puzzle-io-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Transactions API
  slug: puzzle-io-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Ledger Accounts API
  slug: puzzle-io-ledger-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Journal Entries API
  slug: puzzle-io-journal-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Financial Reports API
  slug: puzzle-io-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Metrics API
  slug: puzzle-io-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Categories API
  slug: puzzle-io-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Integrations API
  slug: puzzle-io-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: puzzle.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep 10 13:33:15 2026 GMT
  host: puzzle.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: puzzle-api.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 16:59:42 2026 GMT
  host: staging.southparkdata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Puzzle Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Puzzle, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Puzzle
provider_slug: puzzle-io
slug: puzzle-io-domain-security
source_filename: puzzle-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: puzzle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 13:33:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: puzzle-api.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: staging.southparkdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 16:59:42 2026 GMT\n  hsts: null\ndomains:\n- domain: puzzle.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/security/puzzle-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Accounting
- Fintech
- General Ledger
- Financial Reporting
- Bookkeeping
- Startups
- Embedded Accounting
- Metrics
---
