---
api_specs:
- filename: conductor-admin-api-openapi.yml
  format: yaml
  label: Conductor Admin API
  slug: conductor-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/openapi/conductor-admin-api-openapi.yml
- filename: conductor-event-api-openapi.yml
  format: yaml
  label: Conductor Event API
  slug: conductor-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/openapi/conductor-event-api-openapi.yml
- filename: conductor-metadata-task-api-openapi.yml
  format: yaml
  label: Conductor Metadata - Task API
  slug: conductor-metadata-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/openapi/conductor-metadata-task-api-openapi.yml
- filename: conductor-metadata-workflow-api-openapi.yml
  format: yaml
  label: Conductor Metadata - Workflow API
  slug: conductor-metadata-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/openapi/conductor-metadata-workflow-api-openapi.yml
- filename: conductor-task-api-openapi.yml
  format: yaml
  label: Conductor Task API
  slug: conductor-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/openapi/conductor-task-api-openapi.yml
- filename: conductor-workflow-api-openapi.yml
  format: yaml
  label: Conductor Workflow API
  slug: conductor-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/openapi/conductor-workflow-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: orkes.io
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: play.orkes.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conductor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conductor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Conductor
provider_slug: conductor
slug: conductor-domain-security
source_filename: conductor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: play.orkes.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: orkes.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/security/conductor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Orchestration
- State
- Tasks
- Workflows
---
