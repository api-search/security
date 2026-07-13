---
api_specs:
- filename: docs
  format: yaml
  label: Cognee REST API
  slug: cognee-rest-api
  spec_type: OpenAPI
  url: https://api.cognee.ai/docs
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cognee.ai
  spf: true
hosts:
- cert_expires: Sep 13 08:29:37 2026 GMT
  host: www.cognee.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 09:00:33 2026 GMT
  host: docs.cognee.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.cognee.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Cognee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognee, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cognee
provider_slug: cognee
slug: cognee-domain-security
source_filename: cognee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cognee.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:29:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.cognee.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 09:00:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cognee.ai\n  https: false\ndomains:\n- domain: cognee.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognee/refs/heads/main/security/cognee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Memory
- Knowledge Graph
- RAG
- Agents
- Graph Database
- Vector Search
- LLM
- Open Source
---
