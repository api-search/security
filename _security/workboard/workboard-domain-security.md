---
api_specs:
- filename: workboard-activity-action-items-api-openapi.yml
  format: yaml
  label: WorkBoard Activity (Action Items) API
  slug: workboard-activity-action-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-activity-action-items-api-openapi.yml
- filename: workboard-custom-attributes-api-openapi.yml
  format: yaml
  label: WorkBoard custom-attributes API
  slug: workboard-custom-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-custom-attributes-api-openapi.yml
- filename: workboard-datastream-api-openapi.yml
  format: yaml
  label: WorkBoard Datastream API
  slug: workboard-datastream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-datastream-api-openapi.yml
- filename: workboard-goal-objective-api-openapi.yml
  format: yaml
  label: WorkBoard Goal (Objective) API
  slug: workboard-goal-objective-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-goal-objective-api-openapi.yml
- filename: workboard-metric-key-result-api-openapi.yml
  format: yaml
  label: WorkBoard Metric (Key Result) API
  slug: workboard-metric-key-result-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-metric-key-result-api-openapi.yml
- filename: workboard-tags-api-openapi.yml
  format: yaml
  label: WorkBoard Tags API
  slug: workboard-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-tags-api-openapi.yml
- filename: workboard-team-api-openapi.yml
  format: yaml
  label: WorkBoard Team API
  slug: workboard-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-team-api-openapi.yml
- filename: workboard-user-api-openapi.yml
  format: yaml
  label: WorkBoard User API
  slug: workboard-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-user-api-openapi.yml
- filename: workboard-user-goals-user-objectives-api-openapi.yml
  format: yaml
  label: WorkBoard User Goals (User Objectives) API
  slug: workboard-user-goals-user-objectives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-user-goals-user-objectives-api-openapi.yml
- filename: workboard-webhook-api-openapi.yml
  format: yaml
  label: WorkBoard Webhook API
  slug: workboard-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-webhook-api-openapi.yml
- filename: workboard-workstream-api-openapi.yml
  format: yaml
  label: WorkBoard Workstream API
  slug: workboard-workstream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-workstream-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wobo-int.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: myworkboard.com
  spf: true
hosts:
- cert_expires: Oct  7 08:01:33 2026 GMT
  host: demo.biz.wobo-int.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 19:50:02 2026 GMT
  host: www.myworkboard.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WorkBoard, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: WorkBoard
provider_slug: workboard
slug: workboard-domain-security
source_filename: workboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: demo.biz.wobo-int.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 08:01:33 2026 GMT\n  hsts: null\n- host: www.myworkboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 19:50:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: wobo-int.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: myworkboard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/security/workboard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- OKRs
- Strategy Execution
- Goals
- Key Results
- Enterprise
- AI Agents
- Performance Management
- Strategic Portfolio Management
---
