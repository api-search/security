---
api_specs:
- filename: streak-boxes-api-openapi.yml
  format: yaml
  label: Streak Boxes API
  slug: streak-boxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streak/refs/heads/main/openapi/streak-boxes-api-openapi.yml
- filename: streak-fields-api-openapi.yml
  format: yaml
  label: Streak Fields API
  slug: streak-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streak/refs/heads/main/openapi/streak-fields-api-openapi.yml
- filename: streak-newsfeed-api-openapi.yml
  format: yaml
  label: Streak Newsfeed API
  slug: streak-newsfeed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streak/refs/heads/main/openapi/streak-newsfeed-api-openapi.yml
- filename: streak-pipelines-api-openapi.yml
  format: yaml
  label: Streak Pipelines API
  slug: streak-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streak/refs/heads/main/openapi/streak-pipelines-api-openapi.yml
- filename: streak-stages-api-openapi.yml
  format: yaml
  label: Streak Stages API
  slug: streak-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streak/refs/heads/main/openapi/streak-stages-api-openapi.yml
- filename: streak-users-api-openapi.yml
  format: yaml
  label: Streak Users API
  slug: streak-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streak/refs/heads/main/openapi/streak-users-api-openapi.yml
- filename: streak-webhooks-api-openapi.yml
  format: yaml
  label: Streak Webhooks API
  slug: streak-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streak/refs/heads/main/openapi/streak-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: streak.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep  5 17:50:42 2026 GMT
  host: www.streak.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: streak.readme.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 15:44:14 2026 GMT
  host: api.streak.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Streak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Streak, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Streak
provider_slug: streak
slug: streak-domain-security
source_filename: streak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.streak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 17:50:42 2026 GMT\n  hsts: false\n- host: streak.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: null\n- host: api.streak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 15:44:14 2026 GMT\n  hsts: false\ndomains:\n- domain: streak.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streak/refs/heads/main/security/streak-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CRM
- Sales
- Gmail
- Pipeline Management
- Email Tracking
- Productivity
- Small Business
- Workflows
---
