---
api_specs:
- filename: talend-connections-api-openapi.yml
  format: yaml
  label: Talend Cloud Connections API
  slug: talend-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-connections-api-openapi.yml
- filename: talend-artifacts-api-openapi.yml
  format: yaml
  label: Talend Artifacts API
  slug: talend-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-artifacts-api-openapi.yml
- filename: talend-connections-api-openapi.yml
  format: yaml
  label: Talend Connections API
  slug: talend-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-connections-api-openapi.yml
- filename: talend-environments-api-openapi.yml
  format: yaml
  label: Talend Environments API
  slug: talend-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-environments-api-openapi.yml
- filename: talend-plan-executions-api-openapi.yml
  format: yaml
  label: Talend Plan Executions API
  slug: talend-plan-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-plan-executions-api-openapi.yml
- filename: talend-plans-api-openapi.yml
  format: yaml
  label: Talend Plans API
  slug: talend-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-plans-api-openapi.yml
- filename: talend-promotion-executions-api-openapi.yml
  format: yaml
  label: Talend Promotion Executions API
  slug: talend-promotion-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-promotion-executions-api-openapi.yml
- filename: talend-promotions-api-openapi.yml
  format: yaml
  label: Talend Promotions API
  slug: talend-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-promotions-api-openapi.yml
- filename: talend-remote-engine-clusters-api-openapi.yml
  format: yaml
  label: Talend Remote Engine Clusters API
  slug: talend-remote-engine-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-remote-engine-clusters-api-openapi.yml
- filename: talend-remote-engines-api-openapi.yml
  format: yaml
  label: Talend Remote Engines API
  slug: talend-remote-engines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-remote-engines-api-openapi.yml
- filename: talend-run-profiles-api-openapi.yml
  format: yaml
  label: Talend Run Profiles API
  slug: talend-run-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-run-profiles-api-openapi.yml
- filename: talend-schedules-api-openapi.yml
  format: yaml
  label: Talend Schedules API
  slug: talend-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-schedules-api-openapi.yml
- filename: talend-task-executions-api-openapi.yml
  format: yaml
  label: Talend Task Executions API
  slug: talend-task-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-task-executions-api-openapi.yml
- filename: talend-tasks-api-openapi.yml
  format: yaml
  label: Talend Tasks API
  slug: talend-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-tasks-api-openapi.yml
- filename: talend-workspaces-api-openapi.yml
  format: yaml
  label: Talend Workspaces API
  slug: talend-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: qlik.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: talend.com
  spf: true
hosts:
- cert_expires: Sep 24 02:53:47 2026 GMT
  host: talend.qlik.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 20:15:14 2026 GMT
  host: www.talend.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Talend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Talend, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Talend
provider_slug: talend
slug: talend-domain-security
source_filename: talend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: talend.qlik.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 02:53:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.talend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:15:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: qlik.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: talend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/security/talend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API Management
- Data Integration
- Data Quality
- ETL
- Orchestration
- Pipelines
---
