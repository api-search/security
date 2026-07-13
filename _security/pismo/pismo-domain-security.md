---
api_specs:
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Accounts API
  slug: pismo-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Customers API
  slug: pismo-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Cards API
  slug: pismo-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Authorizations API
  slug: pismo-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Transactions and Statements API
  slug: pismo-transactions-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Programs API
  slug: pismo-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Events API
  slug: pismo-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 iodef "mailto:psm-csirt@pismo.io"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pismo.io
  spf: true
hosts:
- cert_expires: Sep 16 00:41:29 2026 GMT
  host: www.pismo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 16:57:57 2026 GMT
  host: developers.pismo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 14:30:14 2026 GMT
  host: api.pismo.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pismo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pismo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pismo
provider_slug: pismo
slug: pismo-domain-security
source_filename: pismo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pismo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 00:41:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.pismo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 16:57:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pismo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 14:30:14 2026 GMT\n  hsts: null\ndomains:\n- domain: pismo.io\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 iodef \"mailto:psm-csirt@pismo.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/security/pismo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Card Issuing
- Payments
- Fintech
- Core Banking
- Cloud Native
---
