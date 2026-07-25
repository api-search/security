---
api_specs:
- filename: height-activities-api-openapi.yml
  format: yaml
  label: Height Activities API
  slug: height-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/openapi/height-activities-api-openapi.yml
- filename: height-field-templates-api-openapi.yml
  format: yaml
  label: Height Field Templates API
  slug: height-field-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/openapi/height-field-templates-api-openapi.yml
- filename: height-groups-api-openapi.yml
  format: yaml
  label: Height Groups API
  slug: height-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/openapi/height-groups-api-openapi.yml
- filename: height-lists-api-openapi.yml
  format: yaml
  label: Height Lists API
  slug: height-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/openapi/height-lists-api-openapi.yml
- filename: height-security-log-events-api-openapi.yml
  format: yaml
  label: Height Security Log Events API
  slug: height-security-log-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/openapi/height-security-log-events-api-openapi.yml
- filename: height-task-forms-api-openapi.yml
  format: yaml
  label: Height Task Forms API
  slug: height-task-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/openapi/height-task-forms-api-openapi.yml
- filename: height-tasks-api-openapi.yml
  format: yaml
  label: Height Tasks API
  slug: height-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/openapi/height-tasks-api-openapi.yml
- filename: height-users-api-openapi.yml
  format: yaml
  label: Height Users API
  slug: height-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/openapi/height-users-api-openapi.yml
- filename: height-workspace-api-openapi.yml
  format: yaml
  label: Height Workspace API
  slug: height-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/openapi/height-workspace-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: height.app
  spf: true
hosts:
- host: height.app
  https: false
- host: api.height.app
  https: false
kind: domain-security
layout: security
method: probed
name: Height Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Height, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Height
provider_slug: height
slug: height-domain-security
source_filename: height-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: height.app\n  https: false\n- host: api.height.app\n  https: false\ndomains:\n- domain: height.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/security/height-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Project Management
- Task Management
- Collaboration
- Productivity
- Workflow Automation
- AI
---
