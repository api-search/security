---
api_specs:
- filename: hatchet-openapi.yml
  format: yaml
  label: Hatchet API
  slug: hatchet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hatchet/refs/heads/main/openapi/hatchet-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hatchet.run
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: hatchet-cloud.run
  spf: false
hosts:
- cert_expires: Aug 17 02:22:25 2026 GMT
  host: hatchet.run
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 05:54:59 2026 GMT
  host: docs.hatchet.run
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.hatchet-cloud.run
  https: false
kind: domain-security
layout: security
method: probed
name: Hatchet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hatchet, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hatchet
provider_slug: hatchet
slug: hatchet-domain-security
source_filename: hatchet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hatchet.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 02:22:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.hatchet.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 05:54:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hatchet-cloud.run\n  https: false\ndomains:\n- domain: hatchet.run\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: hatchet-cloud.run\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hatchet/refs/heads/main/security/hatchet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Task Queue
- Workflow Engine
- Durable Execution
- Background Tasks
- AI Agents
- Orchestration
- PostgreSQL
- Open Source
---
