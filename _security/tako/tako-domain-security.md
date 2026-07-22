---
api_specs:
- filename: tako-openapi-original.yml
  format: yaml
  label: Tako Knowledge Search API
  slug: tako-knowledge-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tako/refs/heads/main/openapi/tako-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tako.com
  spf: true
hosts:
- cert_expires: Sep  9 08:22:25 2026 GMT
  host: docs.tako.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 17:45:46 2026 GMT
  host: tako.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tako Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tako, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tako
provider_slug: tako
slug: tako-domain-security
source_filename: tako-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.tako.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 08:22:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: tako.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 17:45:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tako.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tako/refs/heads/main/security/tako-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Data
- Search
- Answer Engine
- Financial Data
- Knowledge Graph
- Agents
- MCP
- Data Visualization
---
