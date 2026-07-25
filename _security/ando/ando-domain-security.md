---
api_specs:
- filename: ando-calls-api-openapi.yml
  format: yaml
  label: Ando Calls API
  slug: ando-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ando/refs/heads/main/openapi/ando-calls-api-openapi.yml
- filename: ando-clipboards-api-openapi.yml
  format: yaml
  label: Ando Clipboards API
  slug: ando-clipboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ando/refs/heads/main/openapi/ando-clipboards-api-openapi.yml
- filename: ando-members-api-openapi.yml
  format: yaml
  label: Ando Members API
  slug: ando-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ando/refs/heads/main/openapi/ando-members-api-openapi.yml
- filename: ando-messages-api-openapi.yml
  format: yaml
  label: Ando Messages API
  slug: ando-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ando/refs/heads/main/openapi/ando-messages-api-openapi.yml
- filename: ando-realtime-api-openapi.yml
  format: yaml
  label: Ando Realtime API
  slug: ando-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ando/refs/heads/main/openapi/ando-realtime-api-openapi.yml
- filename: ando-search-api-openapi.yml
  format: yaml
  label: Ando Search API
  slug: ando-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ando/refs/heads/main/openapi/ando-search-api-openapi.yml
- filename: ando-tasks-api-openapi.yml
  format: yaml
  label: Ando Tasks API
  slug: ando-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ando/refs/heads/main/openapi/ando-tasks-api-openapi.yml
- filename: ando-webhooks-api-openapi.yml
  format: yaml
  label: Ando Webhooks API
  slug: ando-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ando/refs/heads/main/openapi/ando-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ando.so
  spf: true
hosts:
- cert_expires: Sep 27 15:50:16 2026 GMT
  host: ando.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 16:46:37 2026 GMT
  host: api.ando.so
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ando Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ando, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Ando
provider_slug: ando
slug: ando-domain-security
source_filename: ando-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ando.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 15:50:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ando.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 16:46:37 2026 GMT\n  hsts: null\ndomains:\n- domain: ando.so\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ando/refs/heads/main/security/ando-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Business Applications
- Messaging
- Team Collaboration
- AI Agents
- Agents
- Developer Tools
- MCP
- Webhooks
- Productivity
---
