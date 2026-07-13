---
api_specs:
- filename: linkup-so-openapi.yml
  format: yaml
  label: Linkup Search API
  slug: linkup-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkup-so/refs/heads/main/openapi/linkup-so-openapi.yml
- filename: linkup-so-openapi.yml
  format: yaml
  label: Linkup Fetch API
  slug: linkup-fetch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkup-so/refs/heads/main/openapi/linkup-so-openapi.yml
- filename: linkup-so-openapi.yml
  format: yaml
  label: Linkup Research API
  slug: linkup-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkup-so/refs/heads/main/openapi/linkup-so-openapi.yml
- filename: linkup-so-openapi.yml
  format: yaml
  label: Linkup Credits API
  slug: linkup-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkup-so/refs/heads/main/openapi/linkup-so-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: linkup.so
  spf: true
hosts:
- cert_expires: Oct  5 00:34:48 2026 GMT
  host: www.linkup.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 16:01:00 2026 GMT
  host: docs.linkup.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 11:33:11 2026 GMT
  host: api.linkup.so
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linkup So Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linkup, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Linkup
provider_slug: linkup-so
slug: linkup-so-domain-security
source_filename: linkup-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.linkup.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 00:34:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.linkup.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 16:01:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.linkup.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:33:11 2026 GMT\n  hsts: null\ndomains:\n- domain: linkup.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkup-so/refs/heads/main/security/linkup-so-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Web Search
- Grounding
- RAG
---
