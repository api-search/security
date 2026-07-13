---
api_specs:
- filename: turbopuffer-openapi.yml
  format: yaml
  label: turbopuffer REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbopuffer/main/openapi/turbopuffer-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: turbopuffer.com
  spf: true
hosts:
- cert_expires: Sep 15 07:21:41 2026 GMT
  host: turbopuffer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 13:46:54 2026 GMT
  host: api.turbopuffer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Turbopuffer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for turbopuffer, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: turbopuffer
provider_slug: turbopuffer
slug: turbopuffer-domain-security
source_filename: turbopuffer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: turbopuffer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 07:21:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.turbopuffer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 13:46:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: turbopuffer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turbopuffer/refs/heads/main/security/turbopuffer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Vector Search
- Full-Text Search
- Hybrid Search
- BM25
- Serverless
- Object Storage
- RAG
- Semantic Search
- AI Infrastructure
- Embeddings
---
