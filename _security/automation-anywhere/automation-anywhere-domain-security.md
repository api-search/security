---
api_specs:
- filename: automation-anywhere-control-room-openapi.yml
  format: yaml
  label: Automation Anywhere Control Room API
  slug: control-room-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/openapi/automation-anywhere-control-room-openapi.yml
- filename: automation-anywhere-bot-deploy-openapi.yml
  format: yaml
  label: Automation Anywhere Bot Deploy API
  slug: bot-deploy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/openapi/automation-anywhere-bot-deploy-openapi.yml
- filename: automation-anywhere-workload-management-openapi.yml
  format: yaml
  label: Automation Anywhere Workload Management API
  slug: workload-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/openapi/automation-anywhere-workload-management-openapi.yml
- filename: automation-anywhere-bot-insight-openapi.yml
  format: yaml
  label: Automation Anywhere Bot Insight API
  slug: bot-insight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/openapi/automation-anywhere-bot-insight-openapi.yml
- filename: automation-anywhere-api-task-execution-openapi.yml
  format: yaml
  label: Automation Anywhere API Task Execution API
  slug: api-task-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/openapi/automation-anywhere-api-task-execution-openapi.yml
- filename: automation-anywhere-credential-vault-openapi.yml
  format: yaml
  label: Automation Anywhere Credential Vault API
  slug: credential-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/openapi/automation-anywhere-credential-vault-openapi.yml
- filename: automation-anywhere-repository-management-openapi.yml
  format: yaml
  label: Automation Anywhere Repository Management API
  slug: repository-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/openapi/automation-anywhere-repository-management-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: automationanywhere.com
  spf: true
hosts:
- cert_expires: Mar 10 01:35:48 2027 GMT
  host: developer.automationanywhere.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 06:15:14 2026 GMT
  host: www.automationanywhere.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 00:01:22 2026 GMT
  host: docs.automationanywhere.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Automation Anywhere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for automation-anywhere, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: automation-anywhere
provider_slug: automation-anywhere
slug: automation-anywhere-domain-security
source_filename: automation-anywhere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.automationanywhere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 01:35:48 2027 GMT\n  hsts: false\n- host: www.automationanywhere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 06:15:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.automationanywhere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 00:01:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: automationanywhere.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/security/automation-anywhere-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags: []
---
