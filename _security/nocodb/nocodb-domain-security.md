---
api_specs:
- filename: swagger.json
  format: json
  label: NocoDB Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://app.nocodb.com/api/v3/swagger.json
- filename: swagger.json
  format: json
  label: NocoDB Meta API
  slug: meta-api
  spec_type: OpenAPI
  url: https://app.nocodb.com/api/v2/meta/bases/{base_id}/swagger.json
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:support@nocodb.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nocodb.com
  spf: true
hosts:
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: nocodb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: app.nocodb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nocodb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NocoDB, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NocoDB
provider_slug: nocodb
slug: nocodb-domain-security
source_filename: nocodb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nocodb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.nocodb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: nocodb.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:support@nocodb.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nocodb/refs/heads/main/security/nocodb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- No-Code
- Low-Code
- Airtable Alternative
- Open Source
- Spreadsheet
- REST API
- Self-Hosted
---
