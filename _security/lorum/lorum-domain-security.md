---
api_specs:
- filename: lorum-accounts-api-openapi.yml
  format: yaml
  label: Lorum Accounts API
  slug: lorum-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-accounts-api-openapi.yml
- filename: lorum-customers-api-openapi.yml
  format: yaml
  label: Lorum Customers API
  slug: lorum-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-customers-api-openapi.yml
- filename: lorum-customers-v2-api-openapi.yml
  format: yaml
  label: Lorum Customers V2 API
  slug: lorum-customers-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-customers-v2-api-openapi.yml
- filename: lorum-documents-api-openapi.yml
  format: yaml
  label: Lorum Documents API
  slug: lorum-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-documents-api-openapi.yml
- filename: lorum-exchange-api-openapi.yml
  format: yaml
  label: Lorum Exchange API
  slug: lorum-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-exchange-api-openapi.yml
- filename: lorum-internal-transfers-api-openapi.yml
  format: yaml
  label: Lorum Internal Transfers API
  slug: lorum-internal-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-internal-transfers-api-openapi.yml
- filename: lorum-oauth-api-openapi.yml
  format: yaml
  label: Lorum Oauth API
  slug: lorum-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-oauth-api-openapi.yml
- filename: lorum-payments-api-openapi.yml
  format: yaml
  label: Lorum Payments API
  slug: lorum-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-payments-api-openapi.yml
- filename: lorum-simulation-api-openapi.yml
  format: yaml
  label: Lorum Simulation API
  slug: lorum-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-simulation-api-openapi.yml
- filename: lorum-transactions-api-openapi.yml
  format: yaml
  label: Lorum Transactions API
  slug: lorum-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lorum.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: fuse.me
  spf: true
hosts:
- cert_expires: Aug 27 17:49:40 2026 GMT
  host: www.lorum.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 05:35:44 2026 GMT
  host: api.fuse.me
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 05:35:44 2026 GMT
  host: api-sandbox.fuse.me
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lorum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lorum, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lorum
provider_slug: lorum
slug: lorum-domain-security
source_filename: lorum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lorum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:49:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fuse.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 05:35:44 2026 GMT\n  hsts: null\n- host: api-sandbox.fuse.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 05:35:44 2026 GMT\n  hsts: null\ndomains:\n- domain: lorum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: fuse.me\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/security/lorum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Payments
- Banking
- Clearing
- Settlement
- Treasury
- Multi-Currency
- Account
- Foreign Exchange
- Webhook
---
