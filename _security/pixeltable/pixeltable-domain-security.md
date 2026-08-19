---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pixeltable.com
  spf: true
hosts:
- cert_expires: Sep 25 22:48:58 2026 GMT
  host: www.pixeltable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 22:48:58 2026 GMT
  host: docs.pixeltable.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 22:48:58 2026 GMT
  host: pixeltable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pixeltable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pixeltable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pixeltable
provider_slug: pixeltable
slug: pixeltable-domain-security
source_filename: pixeltable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pixeltable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 22:48:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pixeltable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 22:48:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: pixeltable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 22:48:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pixeltable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixeltable/refs/heads/main/security/pixeltable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Data
- Multimodal AI
- AI Data Infrastructure
- Vector Search
- Embeddings
- RAG
- Agent Memory
- Model Context Protocol
- Open Source
- Python
- Data Orchestration
- Computed Columns
- Video Processing
- Machine Learning
---
