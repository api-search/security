---
api_specs:
- filename: elementum-access-token-api-openapi.yml
  format: yaml
  label: Elementum Access Token API
  slug: elementum-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-access-token-api-openapi.yml
- filename: elementum-agents-api-openapi.yml
  format: yaml
  label: Elementum Agents API
  slug: elementum-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-agents-api-openapi.yml
- filename: elementum-apps-api-openapi.yml
  format: yaml
  label: Elementum Apps API
  slug: elementum-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-apps-api-openapi.yml
- filename: elementum-attachments-api-openapi.yml
  format: yaml
  label: Elementum Attachments API
  slug: elementum-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-attachments-api-openapi.yml
- filename: elementum-automations-api-openapi.yml
  format: yaml
  label: Elementum Automations API
  slug: elementum-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-automations-api-openapi.yml
- filename: elementum-comments-api-openapi.yml
  format: yaml
  label: Elementum Comments API
  slug: elementum-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-comments-api-openapi.yml
- filename: elementum-domains-api-openapi.yml
  format: yaml
  label: Elementum Domains API
  slug: elementum-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-domains-api-openapi.yml
- filename: elementum-elements-api-openapi.yml
  format: yaml
  label: Elementum Elements API
  slug: elementum-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-elements-api-openapi.yml
- filename: elementum-flows-api-openapi.yml
  format: yaml
  label: Elementum Flows API
  slug: elementum-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-flows-api-openapi.yml
- filename: elementum-groups-api-openapi.yml
  format: yaml
  label: Elementum Groups API
  slug: elementum-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-groups-api-openapi.yml
- filename: elementum-records-api-openapi.yml
  format: yaml
  label: Elementum Records API
  slug: elementum-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-records-api-openapi.yml
- filename: elementum-related-items-api-openapi.yml
  format: yaml
  label: Elementum Related-items API
  slug: elementum-related-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-related-items-api-openapi.yml
- filename: elementum-search-tables-api-openapi.yml
  format: yaml
  label: Elementum Search Tables API
  slug: elementum-search-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-search-tables-api-openapi.yml
- filename: elementum-skills-api-openapi.yml
  format: yaml
  label: Elementum Skills API
  slug: elementum-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-skills-api-openapi.yml
- filename: elementum-tables-api-openapi.yml
  format: yaml
  label: Elementum Tables API
  slug: elementum-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-tables-api-openapi.yml
- filename: elementum-users-api-openapi.yml
  format: yaml
  label: Elementum Users API
  slug: elementum-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-users-api-openapi.yml
- filename: elementum-views-api-openapi.yml
  format: yaml
  label: Elementum Views API
  slug: elementum-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-views-api-openapi.yml
- filename: elementum-watchers-api-openapi.yml
  format: yaml
  label: Elementum Watchers API
  slug: elementum-watchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/openapi/elementum-watchers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elementum.io
  spf: false
hosts:
- cert_expires: Sep 22 13:19:05 2026 GMT
  host: docs.elementum.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: api.elementum.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Elementum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elementum, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Elementum
provider_slug: elementum
slug: elementum-domain-security
source_filename: elementum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.elementum.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:19:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.elementum.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: elementum.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elementum/refs/heads/main/security/elementum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Automation
- Workflow
- Orchestration
- Agents
- Supply Chain
- No-Code
- Enterprise
- Snowflake
---
