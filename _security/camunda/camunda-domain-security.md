---
api_specs:
- filename: camunda-8-api.yml
  format: yaml
  label: Camunda 8 API
  slug: camunda-8-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-8-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: camunda.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: camunda.io
  spf: true
hosts:
- cert_expires: Aug 17 19:15:04 2026 GMT
  host: camunda.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 05:27:52 2026 GMT
  host: docs.camunda.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Camunda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Camunda, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Camunda
provider_slug: camunda
slug: camunda-domain-security
source_filename: camunda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: camunda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 19:15:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.camunda.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 05:27:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: camunda.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: camunda.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/security/camunda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- BPMN
- Business Process Management
- Process Automation
- Workflow
---
