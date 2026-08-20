---
api_specs:
- filename: timeular-activities-api-openapi.yml
  format: yaml
  label: Timeular Activities API
  slug: timeular-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-activities-api-openapi.yml
- filename: timeular-authentication-api-openapi.yml
  format: yaml
  label: Timeular Authentication API
  slug: timeular-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-authentication-api-openapi.yml
- filename: timeular-current-tracking-api-openapi.yml
  format: yaml
  label: Timeular Current Tracking API
  slug: timeular-current-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-current-tracking-api-openapi.yml
- filename: timeular-folders-api-openapi.yml
  format: yaml
  label: Timeular Folders API
  slug: timeular-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-folders-api-openapi.yml
- filename: timeular-leaves-api-openapi.yml
  format: yaml
  label: Timeular Leaves API
  slug: timeular-leaves-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-leaves-api-openapi.yml
- filename: timeular-members-api-openapi.yml
  format: yaml
  label: Timeular Members API
  slug: timeular-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-members-api-openapi.yml
- filename: timeular-reports-api-openapi.yml
  format: yaml
  label: Timeular Reports API
  slug: timeular-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-reports-api-openapi.yml
- filename: timeular-tags-mentions-api-openapi.yml
  format: yaml
  label: Timeular Tags & Mentions API
  slug: timeular-tags-mentions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-tags-mentions-api-openapi.yml
- filename: timeular-time-entries-api-openapi.yml
  format: yaml
  label: Timeular Time Entries API
  slug: timeular-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-time-entries-api-openapi.yml
- filename: timeular-users-api-openapi.yml
  format: yaml
  label: Timeular Users API
  slug: timeular-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-users-api-openapi.yml
- filename: timeular-webhooks-api-openapi.yml
  format: yaml
  label: Timeular Webhooks API
  slug: timeular-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: early.app
  spf: true
hosts:
- cert_expires: Oct  4 14:46:17 2026 GMT
  host: early.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 09:55:52 2026 GMT
  host: developers.early.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: api.early.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Timeular Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Timeular, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Timeular
provider_slug: timeular
slug: timeular-domain-security
source_filename: timeular-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: early.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:46:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.early.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 09:55:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.early.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: early.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/security/timeular-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Time Tracking
- Productivity
- Time Management
- Reporting
- Team Management
- Webhook
- Software-as-a-Service
---
