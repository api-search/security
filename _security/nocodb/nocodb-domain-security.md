---
api_specs:
- filename: nocodb-attachments-api-openapi.yml
  format: yaml
  label: NocoDB Attachments API
  slug: nocodb-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nocodb/refs/heads/main/openapi/nocodb-attachments-api-openapi.yml
- filename: nocodb-auth-api-openapi.yml
  format: yaml
  label: NocoDB Auth API
  slug: nocodb-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nocodb/refs/heads/main/openapi/nocodb-auth-api-openapi.yml
- filename: nocodb-bases-api-openapi.yml
  format: yaml
  label: NocoDB Bases API
  slug: nocodb-bases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nocodb/refs/heads/main/openapi/nocodb-bases-api-openapi.yml
- filename: nocodb-fields-api-openapi.yml
  format: yaml
  label: NocoDB Fields API
  slug: nocodb-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nocodb/refs/heads/main/openapi/nocodb-fields-api-openapi.yml
- filename: nocodb-hooks-api-openapi.yml
  format: yaml
  label: NocoDB Hooks API
  slug: nocodb-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nocodb/refs/heads/main/openapi/nocodb-hooks-api-openapi.yml
- filename: nocodb-links-api-openapi.yml
  format: yaml
  label: NocoDB Links API
  slug: nocodb-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nocodb/refs/heads/main/openapi/nocodb-links-api-openapi.yml
- filename: nocodb-records-api-openapi.yml
  format: yaml
  label: NocoDB Records API
  slug: nocodb-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nocodb/refs/heads/main/openapi/nocodb-records-api-openapi.yml
- filename: nocodb-tables-api-openapi.yml
  format: yaml
  label: NocoDB Tables API
  slug: nocodb-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nocodb/refs/heads/main/openapi/nocodb-tables-api-openapi.yml
- filename: nocodb-views-api-openapi.yml
  format: yaml
  label: NocoDB Views API
  slug: nocodb-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nocodb/refs/heads/main/openapi/nocodb-views-api-openapi.yml
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
