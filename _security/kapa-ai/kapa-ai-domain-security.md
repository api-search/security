---
api_specs:
- filename: kapa-ai-openapi.yml
  format: yaml
  label: kapa.ai Query Chat API
  slug: kapa-ai-query-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kapa-ai/refs/heads/main/openapi/kapa-ai-openapi.yml
- filename: kapa-ai-openapi.yml
  format: yaml
  label: kapa.ai Threads Conversations API
  slug: kapa-ai-threads-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kapa-ai/refs/heads/main/openapi/kapa-ai-openapi.yml
- filename: kapa-ai-openapi.yml
  format: yaml
  label: kapa.ai Search and Retrieval API
  slug: kapa-ai-search-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kapa-ai/refs/heads/main/openapi/kapa-ai-openapi.yml
- filename: kapa-ai-openapi.yml
  format: yaml
  label: kapa.ai Projects API
  slug: kapa-ai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kapa-ai/refs/heads/main/openapi/kapa-ai-openapi.yml
- filename: kapa-ai-openapi.yml
  format: yaml
  label: kapa.ai Analytics API
  slug: kapa-ai-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kapa-ai/refs/heads/main/openapi/kapa-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kapa.ai
  spf: true
hosts:
- cert_expires: Sep 23 15:02:00 2026 GMT
  host: www.kapa.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 09:26:07 2026 GMT
  host: docs.kapa.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 13:13:34 2026 GMT
  host: api.kapa.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kapa Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for kapa.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: kapa.ai
provider_slug: kapa-ai
slug: kapa-ai-domain-security
source_filename: kapa-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kapa.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:02:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.kapa.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 09:26:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.kapa.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 13:13:34 2026 GMT\n  hsts: null\ndomains:\n- domain: kapa.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kapa-ai/refs/heads/main/security/kapa-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Answer Engine
- RAG
- Documentation
- Developer Tools
---
