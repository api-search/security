---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ragflow.io
  spf: true
hosts:
- cert_expires: Nov 11 10:32:19 2026 GMT
  host: ragflow.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 16:54:10 2026 GMT
  host: cloud.ragflow.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ragflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RAGFlow, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RAGFlow
provider_slug: ragflow
slug: ragflow-domain-security
source_filename: ragflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ragflow.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 10:32:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud.ragflow.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 16:54:10 2026 GMT\n  hsts: false\ndomains:\n- domain: ragflow.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ragflow/refs/heads/main/security/ragflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Retrieval Augmented Generation
- Search
- Vector Database
- Document Processing
- Knowledge-Management
- Agents
- Open-Source
- LLM
- MCP
---
