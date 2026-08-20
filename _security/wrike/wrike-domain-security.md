---
api_specs:
- filename: wrike-access-roles-api-openapi.yml
  format: yaml
  label: Wrike Access Roles API
  slug: wrike-access-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-access-roles-api-openapi.yml
- filename: wrike-accounts-api-openapi.yml
  format: yaml
  label: Wrike Accounts API
  slug: wrike-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-accounts-api-openapi.yml
- filename: wrike-colors-api-openapi.yml
  format: yaml
  label: Wrike Colors API
  slug: wrike-colors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-colors-api-openapi.yml
- filename: wrike-comments-api-openapi.yml
  format: yaml
  label: Wrike Comments API
  slug: wrike-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-comments-api-openapi.yml
- filename: wrike-contacts-api-openapi.yml
  format: yaml
  label: Wrike Contacts API
  slug: wrike-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-contacts-api-openapi.yml
- filename: wrike-custom-fields-api-openapi.yml
  format: yaml
  label: Wrike Custom Fields API
  slug: wrike-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-custom-fields-api-openapi.yml
- filename: wrike-folders-and-projects-api-openapi.yml
  format: yaml
  label: Wrike Folders And Projects API
  slug: wrike-folders-and-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-folders-and-projects-api-openapi.yml
- filename: wrike-groups-api-openapi.yml
  format: yaml
  label: Wrike Groups API
  slug: wrike-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-groups-api-openapi.yml
- filename: wrike-tasks-api-openapi.yml
  format: yaml
  label: Wrike Tasks API
  slug: wrike-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-tasks-api-openapi.yml
- filename: wrike-time-logs-api-openapi.yml
  format: yaml
  label: Wrike Time Logs API
  slug: wrike-time-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-time-logs-api-openapi.yml
- filename: wrike-users-api-openapi.yml
  format: yaml
  label: Wrike Users API
  slug: wrike-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-users-api-openapi.yml
- filename: wrike-webhooks-api-openapi.yml
  format: yaml
  label: Wrike Webhooks API
  slug: wrike-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-webhooks-api-openapi.yml
- filename: wrike-workflows-api-openapi.yml
  format: yaml
  label: Wrike Workflows API
  slug: wrike-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wrike.com
  spf: true
hosts:
- cert_expires: Sep 26 14:17:21 2026 GMT
  host: developers.wrike.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 11:30:53 2026 GMT
  host: www.wrike.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wrike Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wrike, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wrike
provider_slug: wrike
slug: wrike-domain-security
source_filename: wrike-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.wrike.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:17:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.wrike.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 11:30:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wrike.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/security/wrike-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Work Management
- Project Management
- Collaboration
- Productivity
- Workflow-Automation
- Task Management
---
