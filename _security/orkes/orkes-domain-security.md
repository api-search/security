---
api_specs:
- filename: orkes-authentication-api-openapi.yml
  format: yaml
  label: Orkes Authentication API
  slug: orkes-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/openapi/orkes-authentication-api-openapi.yml
- filename: orkes-human-tasks-api-openapi.yml
  format: yaml
  label: Orkes Human Tasks API
  slug: orkes-human-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/openapi/orkes-human-tasks-api-openapi.yml
- filename: orkes-schedules-api-openapi.yml
  format: yaml
  label: Orkes Schedules API
  slug: orkes-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/openapi/orkes-schedules-api-openapi.yml
- filename: orkes-secrets-api-openapi.yml
  format: yaml
  label: Orkes Secrets API
  slug: orkes-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/openapi/orkes-secrets-api-openapi.yml
- filename: orkes-task-metadata-api-openapi.yml
  format: yaml
  label: Orkes Task Metadata API
  slug: orkes-task-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/openapi/orkes-task-metadata-api-openapi.yml
- filename: orkes-tasks-api-openapi.yml
  format: yaml
  label: Orkes Tasks API
  slug: orkes-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/openapi/orkes-tasks-api-openapi.yml
- filename: orkes-workflow-execution-api-openapi.yml
  format: yaml
  label: Orkes Workflow Execution API
  slug: orkes-workflow-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/openapi/orkes-workflow-execution-api-openapi.yml
- filename: orkes-workflow-metadata-api-openapi.yml
  format: yaml
  label: Orkes Workflow Metadata API
  slug: orkes-workflow-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/openapi/orkes-workflow-metadata-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: orkes.io
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: orkes.io
  hsts: true
  hsts_max_age: 1800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orkes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orkes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Orkes
provider_slug: orkes
slug: orkes-domain-security
source_filename: orkes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orkes.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 1800\ndomains:\n- domain: orkes.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orkes/refs/heads/main/security/orkes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Microservices
---
