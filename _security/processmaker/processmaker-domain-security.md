---
api_specs:
- filename: processmaker-environment-variables-api-openapi.yml
  format: yaml
  label: ProcessMaker Environment Variables API
  slug: processmaker-environment-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-environment-variables-api-openapi.yml
- filename: processmaker-files-api-openapi.yml
  format: yaml
  label: ProcessMaker Files API
  slug: processmaker-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-files-api-openapi.yml
- filename: processmaker-groups-api-openapi.yml
  format: yaml
  label: ProcessMaker Groups API
  slug: processmaker-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-groups-api-openapi.yml
- filename: processmaker-notifications-api-openapi.yml
  format: yaml
  label: ProcessMaker Notifications API
  slug: processmaker-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-notifications-api-openapi.yml
- filename: processmaker-processes-api-openapi.yml
  format: yaml
  label: ProcessMaker Processes API
  slug: processmaker-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-processes-api-openapi.yml
- filename: processmaker-requests-api-openapi.yml
  format: yaml
  label: ProcessMaker Requests API
  slug: processmaker-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-requests-api-openapi.yml
- filename: processmaker-screens-api-openapi.yml
  format: yaml
  label: ProcessMaker Screens API
  slug: processmaker-screens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-screens-api-openapi.yml
- filename: processmaker-settings-api-openapi.yml
  format: yaml
  label: ProcessMaker Settings API
  slug: processmaker-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-settings-api-openapi.yml
- filename: processmaker-tasks-api-openapi.yml
  format: yaml
  label: ProcessMaker Tasks API
  slug: processmaker-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-tasks-api-openapi.yml
- filename: processmaker-users-api-openapi.yml
  format: yaml
  label: ProcessMaker Users API
  slug: processmaker-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: processmaker.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gitbook.io
  spf: true
hosts:
- cert_expires: Sep  6 23:14:38 2026 GMT
  host: www.processmaker.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 17:00:10 2026 GMT
  host: processmaker.gitbook.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Processmaker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ProcessMaker, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ProcessMaker
provider_slug: processmaker
slug: processmaker-domain-security
source_filename: processmaker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.processmaker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:14:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: processmaker.gitbook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 17:00:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: processmaker.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: gitbook.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/security/processmaker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- BPM
- Business Process Management
- Workflow Automation
- BPMN 2.0
- Low-Code
- Intelligent Automation
- Process Design
- Case Management
- Task Management
- Enterprise Integration
---
