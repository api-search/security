---
api_specs:
- filename: lawvu-contracts-api-openapi.yml
  format: yaml
  label: LawVu Contracts API
  slug: lawvu-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawvu/openapi/lawvu-contracts-api-openapi.yml
- filename: lawvu-fields-api-openapi.yml
  format: yaml
  label: LawVu Fields API
  slug: lawvu-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawvu/openapi/lawvu-fields-api-openapi.yml
- filename: lawvu-files-api-openapi.yml
  format: yaml
  label: LawVu Files API
  slug: lawvu-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawvu/openapi/lawvu-files-api-openapi.yml
- filename: lawvu-invoices-api-openapi.yml
  format: yaml
  label: LawVu Invoices API
  slug: lawvu-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawvu/openapi/lawvu-invoices-api-openapi.yml
- filename: lawvu-matters-api-openapi.yml
  format: yaml
  label: LawVu Matters API
  slug: lawvu-matters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawvu/openapi/lawvu-matters-api-openapi.yml
- filename: lawvu-teams-api-openapi.yml
  format: yaml
  label: LawVu Teams API
  slug: lawvu-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawvu/openapi/lawvu-teams-api-openapi.yml
- filename: lawvu-users-api-openapi.yml
  format: yaml
  label: LawVu Users API
  slug: lawvu-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawvu/openapi/lawvu-users-api-openapi.yml
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
hosts_probed: 3
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
source_yaml_url: https://artifacts.apis.io/lawvu/security/lawvu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Legal
- Legal Tech
- Legal Operations
- Contract Lifecycle Management
- Matter Management
- Document Management
- Spend Management
- Software-as-a-Service
- Workflows
---
