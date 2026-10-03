---
api_specs:
- filename: boomi-atoms-api-openapi.yml
  format: yaml
  label: Boomi Atoms API
  slug: boomi-atoms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-atoms-api-openapi.yml
- filename: boomi-components-api-openapi.yml
  format: yaml
  label: Boomi Components API
  slug: boomi-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-components-api-openapi.yml
- filename: boomi-deployments-api-openapi.yml
  format: yaml
  label: Boomi Deployments API
  slug: boomi-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-deployments-api-openapi.yml
- filename: boomi-environments-api-openapi.yml
  format: yaml
  label: Boomi Environments API
  slug: boomi-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-environments-api-openapi.yml
- filename: boomi-execution-api-openapi.yml
  format: yaml
  label: Boomi Execution API
  slug: boomi-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-execution-api-openapi.yml
- filename: boomi-golden-records-api-openapi.yml
  format: yaml
  label: Boomi Golden Records API
  slug: boomi-golden-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-golden-records-api-openapi.yml
- filename: boomi-messages-api-openapi.yml
  format: yaml
  label: Boomi Messages API
  slug: boomi-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-messages-api-openapi.yml
- filename: boomi-models-api-openapi.yml
  format: yaml
  label: Boomi Models API
  slug: boomi-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-models-api-openapi.yml
- filename: boomi-processes-api-openapi.yml
  format: yaml
  label: Boomi Processes API
  slug: boomi-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-processes-api-openapi.yml
- filename: boomi-quarantine-api-openapi.yml
  format: yaml
  label: Boomi Quarantine API
  slug: boomi-quarantine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-quarantine-api-openapi.yml
- filename: boomi-repositories-api-openapi.yml
  format: yaml
  label: Boomi Repositories API
  slug: boomi-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-repositories-api-openapi.yml
- filename: boomi-sources-api-openapi.yml
  format: yaml
  label: Boomi Sources API
  slug: boomi-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-sources-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: boomi.com
  spf: true
hosts:
- cert_expires: Nov  6 19:31:17 2026 GMT
  host: boomi.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 11:09:06 2026 GMT
  host: help.boomi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 19:48:10 2026 GMT
  host: developer.boomi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Boomi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boomi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Boomi
provider_slug: boomi
slug: boomi-domain-security
source_filename: boomi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boomi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 19:31:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: help.boomi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 11:09:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.boomi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 19:48:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: boomi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/security/boomi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Agents
- Automation
- B2B
- Data Integration
- EDI
- Integration
- iPaaS
- Management
- MFT
- Platform
- Workflows
- Workflow Automation
---
