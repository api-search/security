---
api_specs:
- filename: letta-openapi.json
  format: json
  label: Letta Cloud API
  slug: cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta/refs/heads/main/openapi/letta-openapi.json
- filename: letta-openapi.json
  format: json
  label: Letta Self-Hosted Server
  slug: self-hosted
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta/refs/heads/main/openapi/letta-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: letta.com
  spf: true
hosts:
- cert_expires: Sep  9 21:50:59 2026 GMT
  host: www.letta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 20:28:09 2026 GMT
  host: docs.letta.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 01:41:01 2026 GMT
  host: api.letta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Letta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Letta, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Letta
provider_slug: letta
slug: letta-domain-security
source_filename: letta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.letta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 21:50:59 2026 GMT\n  hsts: false\n- host: docs.letta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 20:28:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.letta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 01:41:01 2026 GMT\n  hsts: false\ndomains:\n- domain: letta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/letta/refs/heads/main/security/letta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Agents
- Stateful Agents
- Memory
- MemGPT
- Continual Learning
- MCP
- Multi-Agent
- RAG
- Open Source
---
