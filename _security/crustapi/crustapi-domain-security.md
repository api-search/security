---
api_specs:
- filename: crustapi-demo-api-openapi.yml
  format: yaml
  label: CrustAPI Demo API
  slug: crustapi-demo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crustapi/refs/heads/main/openapi/crustapi-demo-api-openapi.yml
- filename: crustapi-search-api-openapi.yml
  format: yaml
  label: CrustAPI Search API
  slug: crustapi-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crustapi/refs/heads/main/openapi/crustapi-search-api-openapi.yml
- filename: crustapi-linked-in-api-openapi.yml
  format: yaml
  label: CrustAPI Linked In API
  slug: crustapi-linked-in-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crustapi/refs/heads/main/openapi/crustapi-linked-in-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: crustapi.com
  spf: true
hosts:
- cert_expires: Dec  2 23:40:28 2026 GMT
  host: crustapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crustapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CrustAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CrustAPI
provider_slug: crustapi
slug: crustapi-domain-security
source_filename: crustapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crustapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:40:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: crustapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crustapi/refs/heads/main/security/crustapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- Google Maps
- LinkedIn
- SERP / Web Scraping
- Business & Lead Data
- People / Recruiting Data
- Data Enrichment
- AI Agents / MCP
- RAG
- Data
---
