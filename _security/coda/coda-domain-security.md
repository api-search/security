---
api_specs:
- filename: coda-openapi.json
  format: json
  label: Coda Docs API
  slug: coda-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-openapi.json
- filename: coda-openapi.json
  format: json
  label: Coda Folders API
  slug: coda-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-openapi.json
- filename: coda-openapi.json
  format: json
  label: Coda Pages API
  slug: coda-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-openapi.json
- filename: coda-openapi.json
  format: json
  label: Coda Tables API
  slug: coda-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-openapi.json
- filename: coda-openapi.json
  format: json
  label: Coda Columns API
  slug: coda-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-openapi.json
- filename: coda-openapi.json
  format: json
  label: Coda Rows API
  slug: coda-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-openapi.json
- filename: coda-openapi.json
  format: json
  label: Coda Formulas API
  slug: coda-formulas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-openapi.json
- filename: coda-openapi.json
  format: json
  label: Coda Controls API
  slug: coda-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-openapi.json
- filename: coda-openapi.json
  format: json
  label: Coda Automations API
  slug: coda-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-openapi.json
- filename: coda-openapi.json
  format: json
  label: Coda Permissions API
  slug: coda-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-openapi.json
- filename: coda-openapi.json
  format: json
  label: Coda Publishing API
  slug: coda-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-openapi.json
- filename: coda-openapi.json
  format: json
  label: Coda Account API
  slug: coda-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-openapi.json
- filename: coda-openapi.json
  format: json
  label: Coda Analytics API
  slug: coda-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-openapi.json
- filename: coda-openapi.json
  format: json
  label: Coda Packs SDK
  slug: coda-packs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@coda.io"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coda.io
  spf: true
hosts:
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: coda.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coda, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coda
provider_slug: coda
slug: coda-domain-security
source_filename: coda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coda.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: coda.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@coda.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/security/coda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Productivity
- Docs
- No-Code
- Collaboration
- Database
---
