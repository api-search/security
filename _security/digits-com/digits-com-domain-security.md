---
api_specs:
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Transactions API
  slug: digits-com-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Source Sync API
  slug: digits-com-source-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Parties API
  slug: digits-com-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Chart of Accounts API
  slug: digits-com-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Financial Statements API
  slug: digits-com-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Connections API
  slug: digits-com-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Organizations API
  slug: digits-com-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: digits.com
  spf: true
hosts:
- cert_expires: Sep 23 01:42:47 2026 GMT
  host: digits.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 17:15:38 2026 GMT
  host: developer.digits.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 00:55:24 2026 GMT
  host: connect.digits.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Digits Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digits, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Digits
provider_slug: digits-com
slug: digits-com-domain-security
source_filename: digits-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 01:42:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.digits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 17:15:38 2026 GMT\n  hsts: null\n- host: connect.digits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 00:55:24 2026 GMT\n  hsts: null\ndomains:\n- domain: digits.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/security/digits-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Accounting
- Bookkeeping
- Finance
- General Ledger
- AI
- FinTech
---
