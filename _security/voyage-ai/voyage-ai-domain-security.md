---
api_specs:
- filename: llms.txt
  format: yaml
  label: Voyage AI Embeddings API
  slug: embeddings
  spec_type: OpenAPI
  url: https://docs.voyageai.com/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: voyageai.com
  spf: true
hosts:
- cert_expires: Sep 20 00:20:36 2026 GMT
  host: www.voyageai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 01:42:43 2026 GMT
  host: docs.voyageai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 22:51:55 2026 GMT
  host: api.voyageai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Voyage Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voyage AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Voyage AI
provider_slug: voyage-ai
slug: voyage-ai-domain-security
source_filename: voyage-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.voyageai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 00:20:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.voyageai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 01:42:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.voyageai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 22:51:55 2026 GMT\n  hsts: null\ndomains:\n- domain: voyageai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voyage-ai/refs/heads/main/security/voyage-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Embeddings
- Rerankers
- RAG
- Semantic Search
- AI Models
- Vector Search
- Multimodal
---
