---
api_specs:
- filename: nomic-ai-openapi.yml
  format: yaml
  label: Nomic Atlas API
  slug: atlas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomic-ai/refs/heads/main/openapi/nomic-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nomic.ai
  spf: true
hosts:
- cert_expires: Aug 13 00:40:07 2026 GMT
  host: www.nomic.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 06:50:22 2026 GMT
  host: docs.nomic.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: api-atlas.nomic.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nomic Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nomic AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nomic AI
provider_slug: nomic-ai
slug: nomic-ai-domain-security
source_filename: nomic-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nomic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 00:40:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.nomic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 06:50:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-atlas.nomic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nomic.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nomic-ai/refs/heads/main/security/nomic-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Embeddings
- Vector Database
- Data Exploration
- LLM
- Open Source
- RAG
- Atlas
---
