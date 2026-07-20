---
api_specs:
- filename: lawvu-api-openapi-original.yml
  format: yaml
  label: LawVu API
  slug: lawvu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lawvu/refs/heads/main/openapi/lawvu-api-openapi-original.yml
- filename: lawvu-account-openapi-original.json
  format: json
  label: LawVu Account
  slug: lawvu-account
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lawvu/refs/heads/main/openapi/lawvu-account-openapi-original.json
- filename: lawvu-matters-openapi-original.json
  format: json
  label: LawVu Matters
  slug: lawvu-matters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lawvu/refs/heads/main/openapi/lawvu-matters-openapi-original.json
- filename: lawvu-contracts-openapi-original.json
  format: json
  label: LawVu Contracts
  slug: lawvu-contracts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lawvu/refs/heads/main/openapi/lawvu-contracts-openapi-original.json
- filename: lawvu-fields-openapi-original.json
  format: json
  label: LawVu Fields
  slug: lawvu-fields
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lawvu/refs/heads/main/openapi/lawvu-fields-openapi-original.json
- filename: lawvu-files-openapi-original.json
  format: json
  label: LawVu Files
  slug: lawvu-files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lawvu/refs/heads/main/openapi/lawvu-files-openapi-original.json
- filename: lawvu-invoices-openapi-original.json
  format: json
  label: LawVu Invoices
  slug: lawvu-invoices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lawvu/refs/heads/main/openapi/lawvu-invoices-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lawvu.com
  spf: true
hosts:
- cert_expires: Oct  2 13:38:09 2026 GMT
  host: lawvu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 13:32:37 2026 GMT
  host: api-sandbox.lawvu.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 04:13:19 2026 GMT
  host: api.lawvu.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lawvu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LawVu, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LawVu
provider_slug: lawvu
slug: lawvu-domain-security
source_filename: lawvu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lawvu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 13:38:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-sandbox.lawvu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 13:32:37 2026 GMT\n  hsts: null\n- host: api.lawvu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 04:13:19 2026 GMT\n  hsts: null\ndomains:\n- domain: lawvu.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lawvu/refs/heads/main/security/lawvu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Legal
- Legal Technology
- Legal Operations
- Contract Lifecycle Management
- Matter Management
- Document Management
- Spend Management
- SaaS
- Workflow
---
