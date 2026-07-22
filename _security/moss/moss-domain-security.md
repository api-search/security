---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: moss.dev
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: usemoss.dev
  spf: false
hosts:
- cert_expires: Sep  1 18:13:06 2026 GMT
  host: www.moss.dev
  hsts: true
  hsts_max_age: 30
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 17:23:01 2026 GMT
  host: docs.moss.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: service.usemoss.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moss, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Moss
provider_slug: moss
slug: moss-domain-security
source_filename: moss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moss.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 18:13:06 2026 GMT\n  hsts: true\n  hsts_max_age: 30\n- host: docs.moss.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 17:23:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: service.usemoss.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: moss.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: usemoss.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moss/refs/heads/main/security/moss-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Semantic Search
- Vector Search
- Retrieval
- AI Agents
- Voice AI
- Embeddings
- RAG
- Developer Tools
- On-Device AI
---
