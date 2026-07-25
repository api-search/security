---
api_specs:
- filename: bytebase-auth-api-openapi.yml
  format: yaml
  label: Bytebase Auth API
  slug: bytebase-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-auth-api-openapi.yml
- filename: bytebase-databases-api-openapi.yml
  format: yaml
  label: Bytebase Databases API
  slug: bytebase-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-databases-api-openapi.yml
- filename: bytebase-groups-api-openapi.yml
  format: yaml
  label: Bytebase Groups API
  slug: bytebase-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-groups-api-openapi.yml
- filename: bytebase-instances-api-openapi.yml
  format: yaml
  label: Bytebase Instances API
  slug: bytebase-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-instances-api-openapi.yml
- filename: bytebase-issues-api-openapi.yml
  format: yaml
  label: Bytebase Issues API
  slug: bytebase-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-issues-api-openapi.yml
- filename: bytebase-plans-api-openapi.yml
  format: yaml
  label: Bytebase Plans API
  slug: bytebase-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-plans-api-openapi.yml
- filename: bytebase-projects-api-openapi.yml
  format: yaml
  label: Bytebase Projects API
  slug: bytebase-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-projects-api-openapi.yml
- filename: bytebase-roles-api-openapi.yml
  format: yaml
  label: Bytebase Roles API
  slug: bytebase-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-roles-api-openapi.yml
- filename: bytebase-rollouts-api-openapi.yml
  format: yaml
  label: Bytebase Rollouts API
  slug: bytebase-rollouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-rollouts-api-openapi.yml
- filename: bytebase-sheets-api-openapi.yml
  format: yaml
  label: Bytebase Sheets API
  slug: bytebase-sheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-sheets-api-openapi.yml
- filename: bytebase-users-api-openapi.yml
  format: yaml
  label: Bytebase Users API
  slug: bytebase-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-users-api-openapi.yml
- filename: bytebase-webhooks-api-openapi.yml
  format: yaml
  label: Bytebase Webhooks API
  slug: bytebase-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytebase/refs/heads/main/openapi/bytebase-webhooks-api-openapi.yml
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
