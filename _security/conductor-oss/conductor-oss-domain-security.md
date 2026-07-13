---
api_specs:
- filename: conductor-oss-openapi.yml
  format: yaml
  label: Conductor OSS REST API
  slug: conductor-oss-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conductor-oss/refs/heads/main/openapi/conductor-oss-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: conductor-oss.org
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: orkes.io
  spf: true
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: conductor-oss.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 23:22:47 2026 GMT
  host: cloud.orkes.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: docs.conductor-oss.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conductor Oss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conductor OSS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Conductor OSS
provider_slug: conductor-oss
slug: conductor-oss-domain-security
source_filename: conductor-oss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conductor-oss.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: false\n- host: cloud.orkes.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:22:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.conductor-oss.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: conductor-oss.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: orkes.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conductor-oss/refs/heads/main/security/conductor-oss-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agentic AI
- Durable Execution
- Event-Driven
- Microservices
- Netflix
- Open Source
- Orchestration
- Workflow Engine
- Workflows
---
