---
api_specs:
- filename: clickup-tasks-openapi.yml
  format: yaml
  label: ClickUp Tasks API
  slug: tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-tasks-openapi.yml
- filename: clickup-spaces-openapi.yml
  format: yaml
  label: ClickUp Spaces API
  slug: spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-spaces-openapi.yml
- filename: clickup-lists-openapi.yml
  format: yaml
  label: ClickUp Lists API
  slug: lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-lists-openapi.yml
- filename: clickup-folders-openapi.yml
  format: yaml
  label: ClickUp Folders API
  slug: folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-folders-openapi.yml
- filename: clickup-goals-openapi.yml
  format: yaml
  label: ClickUp Goals API
  slug: goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-goals-openapi.yml
- filename: clickup-comments-openapi.yml
  format: yaml
  label: ClickUp Comments API
  slug: comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-comments-openapi.yml
- filename: clickup-teams-openapi.yml
  format: yaml
  label: ClickUp Teams (Workspaces) API
  slug: teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-teams-openapi.yml
- filename: clickup-webhooks-openapi.yml
  format: yaml
  label: ClickUp Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-webhooks-openapi.yml
- filename: clickup-custom-fields-openapi.yml
  format: yaml
  label: ClickUp Custom Fields API
  slug: custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-custom-fields-openapi.yml
- filename: clickup-time-tracking-openapi.yml
  format: yaml
  label: ClickUp Time Tracking API
  slug: time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-time-tracking-openapi.yml
- filename: clickup-views-openapi.yml
  format: yaml
  label: ClickUp Views API
  slug: views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-views-openapi.yml
- filename: clickup-oauth-openapi.yml
  format: yaml
  label: ClickUp OAuth API
  slug: oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-oauth-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clickup.com
  spf: true
hosts:
- cert_expires: Sep 17 04:27:19 2026 GMT
  host: developer.clickup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api.clickup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clickup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for clickup, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: clickup
provider_slug: clickup
slug: clickup-domain-security
source_filename: clickup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.clickup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 04:27:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.clickup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: clickup.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/security/clickup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
