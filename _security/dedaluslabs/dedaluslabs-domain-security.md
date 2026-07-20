---
api_specs:
- filename: dedaluslabs-agents-openapi-original.json
  format: json
  label: Dedalus Agents API
  slug: dedalus-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dedaluslabs/refs/heads/main/openapi/dedaluslabs-agents-openapi-original.json
- filename: dedaluslabs-machines-openapi-original.yml
  format: yaml
  label: Dedalus Cloud Services (Machines) API
  slug: dedalus-cloud-services-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dedaluslabs/refs/heads/main/openapi/dedaluslabs-machines-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: dedaluslabs.ai
  spf: true
hosts:
- cert_expires: Oct  5 11:47:08 2026 GMT
  host: dedaluslabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 20:01:40 2026 GMT
  host: api.dedaluslabs.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 22:37:56 2026 GMT
  host: dcs.dedaluslabs.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dedaluslabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dedalus Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Dedalus Labs
provider_slug: dedaluslabs
slug: dedaluslabs-domain-security
source_filename: dedaluslabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dedaluslabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 11:47:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.dedaluslabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 20:01:40 2026 GMT\n  hsts: null\n- host: dcs.dedaluslabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 22:37:56 2026 GMT\n  hsts: false\ndomains:\n- domain: dedaluslabs.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dedaluslabs/refs/heads/main/security/dedaluslabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Agents
- MCP
- Model Context Protocol
- LLM
- Inference
- Gateway
- Compute
- Sandbox
- Developer Tools
---
