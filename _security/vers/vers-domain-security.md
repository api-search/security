---
api_specs:
- filename: vers-openapi-original.json
  format: json
  label: Vers Orchestrator Control Plane API
  slug: vers-orchestrator-control-plane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vers.sh
  spf: true
hosts:
- cert_expires: Sep 15 16:26:08 2026 GMT
  host: vers.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 16:19:43 2026 GMT
  host: docs.vers.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 21:07:28 2026 GMT
  host: api.vers.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vers, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Vers
provider_slug: vers
slug: vers-domain-security
source_filename: vers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vers.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:26:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.vers.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:19:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.vers.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 21:07:28 2026 GMT\n  hsts: false\ndomains:\n- domain: vers.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/security/vers-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Compute
- Virtualization
- MicroVM
- Orchestration
- Infrastructure
- AI Agents
- Developer Tools
- Sandbox
- CI/CD
---
