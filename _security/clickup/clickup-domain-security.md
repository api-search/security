---
api_specs:
- filename: clickup-authorization-api-openapi.yml
  format: yaml
  label: clickup Authorization API
  slug: clickup-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-authorization-api-openapi.yml
- filename: clickup-comments-api-openapi.yml
  format: yaml
  label: clickup Comments API
  slug: clickup-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-comments-api-openapi.yml
- filename: clickup-custom-fields-api-openapi.yml
  format: yaml
  label: clickup Custom Fields API
  slug: clickup-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-custom-fields-api-openapi.yml
- filename: clickup-folders-api-openapi.yml
  format: yaml
  label: clickup Folders API
  slug: clickup-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-folders-api-openapi.yml
- filename: clickup-goals-api-openapi.yml
  format: yaml
  label: clickup Goals API
  slug: clickup-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-goals-api-openapi.yml
- filename: clickup-lists-api-openapi.yml
  format: yaml
  label: clickup Lists API
  slug: clickup-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-lists-api-openapi.yml
- filename: clickup-oauth-api-openapi.yml
  format: yaml
  label: clickup OAuth API
  slug: clickup-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-oauth-api-openapi.yml
- filename: clickup-spaces-api-openapi.yml
  format: yaml
  label: clickup Spaces API
  slug: clickup-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-spaces-api-openapi.yml
- filename: clickup-tasks-api-openapi.yml
  format: yaml
  label: clickup Tasks API
  slug: clickup-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-tasks-api-openapi.yml
- filename: clickup-teams-api-openapi.yml
  format: yaml
  label: clickup Teams API
  slug: clickup-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-teams-api-openapi.yml
- filename: clickup-time-tracking-api-openapi.yml
  format: yaml
  label: clickup Time Tracking API
  slug: clickup-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-time-tracking-api-openapi.yml
- filename: clickup-views-api-openapi.yml
  format: yaml
  label: clickup Views API
  slug: clickup-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-views-api-openapi.yml
- filename: clickup-webhooks-api-openapi.yml
  format: yaml
  label: clickup Webhooks API
  slug: clickup-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-webhooks-api-openapi.yml
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
