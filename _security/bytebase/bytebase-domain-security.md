---
api_specs:
- filename: bytebase-openapi.yml
  format: yaml
  label: Bytebase Instances API
  slug: instances
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-openapi.yml
- filename: bytebase-openapi.yml
  format: yaml
  label: Bytebase Databases API
  slug: databases
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-openapi.yml
- filename: bytebase-openapi.yml
  format: yaml
  label: Bytebase Projects API
  slug: projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-openapi.yml
- filename: bytebase-openapi.yml
  format: yaml
  label: Bytebase Issues / Migrations API
  slug: issues-migrations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-openapi.yml
- filename: bytebase-openapi.yml
  format: yaml
  label: Bytebase Rollouts API
  slug: rollouts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-openapi.yml
- filename: bytebase-openapi.yml
  format: yaml
  label: Bytebase Sheets API
  slug: sheets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-openapi.yml
- filename: bytebase-openapi.yml
  format: yaml
  label: Bytebase Users / Roles API
  slug: users-roles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-openapi.yml
- filename: bytebase-openapi.yml
  format: yaml
  label: Bytebase Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bytebase.com
  spf: true
hosts:
- cert_expires: Sep 20 13:15:27 2026 GMT
  host: www.bytebase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 14:56:34 2026 GMT
  host: docs.bytebase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: demo.bytebase.com
  https: false
kind: domain-security
layout: security
method: probed
name: Bytebase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bytebase, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bytebase
provider_slug: bytebase
slug: bytebase-domain-security
source_filename: bytebase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bytebase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 13:15:27 2026 GMT\n  hsts: false\n- host: docs.bytebase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 14:56:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: demo.bytebase.com\n  https: false\ndomains:\n- domain: bytebase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/security/bytebase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- DevOps
- Schema Migration
- CI/CD
- DevSecOps
---
