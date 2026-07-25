---
api_specs:
- filename: todoist-sync-api-openapi.yml
  format: yaml
  label: Todoist Sync API v9
  slug: todoist-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-sync-api-openapi.yml
- filename: todoist-comments-api-openapi.yml
  format: yaml
  label: Todoist Comments API
  slug: todoist-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-comments-api-openapi.yml
- filename: todoist-labels-api-openapi.yml
  format: yaml
  label: Todoist Labels API
  slug: todoist-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-labels-api-openapi.yml
- filename: todoist-projects-api-openapi.yml
  format: yaml
  label: Todoist Projects API
  slug: todoist-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-projects-api-openapi.yml
- filename: todoist-reminders-api-openapi.yml
  format: yaml
  label: Todoist Reminders API
  slug: todoist-reminders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-reminders-api-openapi.yml
- filename: todoist-sections-api-openapi.yml
  format: yaml
  label: Todoist Sections API
  slug: todoist-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-sections-api-openapi.yml
- filename: todoist-sync-api-openapi.yml
  format: yaml
  label: Todoist Sync API
  slug: todoist-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-sync-api-openapi.yml
- filename: todoist-tasks-api-openapi.yml
  format: yaml
  label: Todoist Tasks API
  slug: todoist-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-tasks-api-openapi.yml
- filename: todoist-user-api-openapi.yml
  format: yaml
  label: Todoist User API
  slug: todoist-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-user-api-openapi.yml
- filename: todoist-workspaces-api-openapi.yml
  format: yaml
  label: Todoist Workspaces API
  slug: todoist-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-workspaces-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 iodef "mailto:aws.ops@doist.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: todoist.com
  spf: true
hosts:
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: todoist.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: developer.todoist.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: api.todoist.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Todoist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Todoist, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Todoist
provider_slug: todoist
slug: todoist-domain-security
source_filename: todoist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: todoist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.todoist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: false\n- host: api.todoist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: todoist.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 iodef \"mailto:aws.ops@doist.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/security/todoist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Productivity
- Tasks
- To-Do
- Task Management
- Collaboration
---
