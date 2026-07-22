---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.org"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: topk.io
  spf: true
hosts:
- cert_expires: Aug 30 15:21:35 2026 GMT
  host: docs.topk.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: elastica.api.topk.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Topk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Topk, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Topk
provider_slug: topk
slug: topk-domain-security
source_filename: topk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.topk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 15:21:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: elastica.api.topk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: topk.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.org\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/topk/refs/heads/main/security/topk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Search
- Vector Search
- Hybrid Search
- Multi-Vector Retrieval
- Semantic Search
- BM25
- Retrieval
- RAG
- Question Answering
- AI Infrastructure
- Embeddings
- MCP
---
