---
api_specs:
- filename: robocorp-assets-api-openapi.yml
  format: yaml
  label: Robocorp Assets API
  slug: robocorp-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-assets-api-openapi.yml
- filename: robocorp-assistants-api-openapi.yml
  format: yaml
  label: Robocorp Assistants API
  slug: robocorp-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-assistants-api-openapi.yml
- filename: robocorp-process-runs-api-openapi.yml
  format: yaml
  label: Robocorp Process Runs API
  slug: robocorp-process-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-process-runs-api-openapi.yml
- filename: robocorp-processes-api-openapi.yml
  format: yaml
  label: Robocorp Processes API
  slug: robocorp-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-processes-api-openapi.yml
- filename: robocorp-step-runs-api-openapi.yml
  format: yaml
  label: Robocorp Step Runs API
  slug: robocorp-step-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-step-runs-api-openapi.yml
- filename: robocorp-task-packages-api-openapi.yml
  format: yaml
  label: Robocorp Task Packages API
  slug: robocorp-task-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-task-packages-api-openapi.yml
- filename: robocorp-vault-api-openapi.yml
  format: yaml
  label: Robocorp Vault API
  slug: robocorp-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-vault-api-openapi.yml
- filename: robocorp-webhooks-api-openapi.yml
  format: yaml
  label: Robocorp Webhooks API
  slug: robocorp-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-webhooks-api-openapi.yml
- filename: robocorp-work-items-api-openapi.yml
  format: yaml
  label: Robocorp Work Items API
  slug: robocorp-work-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-work-items-api-openapi.yml
- filename: robocorp-worker-groups-api-openapi.yml
  format: yaml
  label: Robocorp Worker Groups API
  slug: robocorp-worker-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-worker-groups-api-openapi.yml
- filename: robocorp-workers-api-openapi.yml
  format: yaml
  label: Robocorp Workers API
  slug: robocorp-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-workers-api-openapi.yml
- filename: robocorp-workspace-api-openapi.yml
  format: yaml
  label: Robocorp Workspace API
  slug: robocorp-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-workspace-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: robocorp.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: rpaframework.org
  spf: true
hosts:
- cert_expires: Sep 19 20:17:39 2026 GMT
  host: robocorp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: cloud.robocorp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 19:06:22 2026 GMT
  host: rpaframework.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Robocorp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Robocorp, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Robocorp
provider_slug: robocorp
slug: robocorp-domain-security
source_filename: robocorp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: robocorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 20:17:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.robocorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rpaframework.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 19:06:22 2026 GMT\n  hsts: false\ndomains:\n- domain: robocorp.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: rpaframework.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/security/robocorp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- RPA
- Workflow-Automation
- Python
- Open-Source
- Automation
---
