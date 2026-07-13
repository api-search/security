---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: getzep.com
  spf: true
hosts:
- cert_expires: Sep 27 19:26:38 2026 GMT
  host: www.getzep.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 15:36:15 2026 GMT
  host: help.getzep.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 15:36:15 2026 GMT
  host: api.getzep.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zep, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Zep
provider_slug: zep
slug: zep-domain-security
source_filename: zep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getzep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 19:26:38 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: help.getzep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 15:36:15 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.getzep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 15:36:15 2026 GMT\n  hsts: null\ndomains:\n- domain: getzep.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zep/refs/heads/main/security/zep-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Memory
- AI Agents
- Knowledge Graph
- Temporal Graph
- Graph RAG
- Context Engineering
- LangChain
- LlamaIndex
- CrewAI
- LLMs
- Personalization
- Retrieval
---
