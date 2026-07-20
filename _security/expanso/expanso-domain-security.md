---
api_specs:
- filename: bacalhau-openapi-original.json
  format: json
  label: Bacalhau Orchestrator API
  slug: bacalhau-orchestrator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expanso/refs/heads/main/openapi/bacalhau-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bacalhau.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: expanso.io
  spf: true
hosts:
- cert_expires: Oct  5 20:07:53 2026 GMT
  host: bacalhau.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: cloud.expanso.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Expanso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Expanso, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Expanso
provider_slug: expanso
slug: expanso-domain-security
source_filename: expanso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bacalhau.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:07:53 2026 GMT\n  hsts: false\n- host: cloud.expanso.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bacalhau.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: expanso.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expanso/refs/heads/main/security/expanso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Distributed Computing
- Edge Computing
- Compute Orchestration
- Data Pipelines
- Data Governance
- Open Source
- AI
- Job Orchestration
---
