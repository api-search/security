---
api_specs:
- filename: external-v1-openapi-original.yml
  format: yaml
  label: WorkBoard External API v1
  slug: workboard-external-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/external-v1-openapi-original.yml
- filename: public-v2-openapi-original.yml
  format: yaml
  label: WorkBoard Public API v2
  slug: workboard-public-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/public-v2-openapi-original.yml
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
