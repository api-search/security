---
api_specs:
- filename: exec-collections-api-openapi.yml
  format: yaml
  label: Exec Collections API
  slug: exec-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-collections-api-openapi.yml
- filename: exec-knowledge-hub-folders-api-openapi.yml
  format: yaml
  label: Exec Knowledge Hub - Folders API
  slug: exec-knowledge-hub-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-knowledge-hub-folders-api-openapi.yml
- filename: exec-knowledge-hub-pages-api-openapi.yml
  format: yaml
  label: Exec Knowledge Hub - Pages API
  slug: exec-knowledge-hub-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-knowledge-hub-pages-api-openapi.yml
- filename: exec-knowledge-hub-sources-api-openapi.yml
  format: yaml
  label: Exec Knowledge Hub - Sources API
  slug: exec-knowledge-hub-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-knowledge-hub-sources-api-openapi.yml
- filename: exec-scenario-studio-api-openapi.yml
  format: yaml
  label: Exec Scenario Studio API
  slug: exec-scenario-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-scenario-studio-api-openapi.yml
- filename: exec-scenarios-api-openapi.yml
  format: yaml
  label: Exec Scenarios API
  slug: exec-scenarios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-scenarios-api-openapi.yml
- filename: exec-sessions-api-openapi.yml
  format: yaml
  label: Exec Sessions API
  slug: exec-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-sessions-api-openapi.yml
- filename: exec-skills-api-openapi.yml
  format: yaml
  label: Exec Skills API
  slug: exec-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-skills-api-openapi.yml
- filename: exec-workspace-api-openapi.yml
  format: yaml
  label: Exec Workspace API
  slug: exec-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-workspace-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: exec.com
  spf: true
hosts:
- cert_expires: Oct 29 17:04:17 2026 GMT
  host: www.exec.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 17:04:17 2026 GMT
  host: docs.exec.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 17:04:17 2026 GMT
  host: api.exec.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exec, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Exec
provider_slug: exec
slug: exec-domain-security
source_filename: exec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.exec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 17:04:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.exec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 17:04:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.exec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 17:04:17 2026 GMT\n  hsts: null\ndomains:\n- domain: exec.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/security/exec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Sales Enablement
- Training
- Roleplay
- Coaching
- Learning
- Knowledge Management
- LMS
---
