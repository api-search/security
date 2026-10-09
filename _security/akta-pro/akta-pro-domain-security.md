---
api_specs:
- filename: akta-pro-company-api-openapi.yml
  format: yaml
  label: akta.pro Company API
  slug: akta-pro-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akta-pro/refs/heads/main/openapi/akta-pro-company-api-openapi.yml
- filename: akta-pro-list-generation-api-openapi.yml
  format: yaml
  label: akta.pro List Generation API
  slug: akta-pro-list-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akta-pro/refs/heads/main/openapi/akta-pro-list-generation-api-openapi.yml
- filename: akta-pro-news-api-openapi.yml
  format: yaml
  label: akta.pro News API
  slug: akta-pro-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akta-pro/refs/heads/main/openapi/akta-pro-news-api-openapi.yml
- filename: akta-pro-reviews-api-openapi.yml
  format: yaml
  label: akta.pro Reviews API
  slug: akta-pro-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akta-pro/refs/heads/main/openapi/akta-pro-reviews-api-openapi.yml
- filename: akta-pro-supporting-apis-api-openapi.yml
  format: yaml
  label: akta.pro Supporting APIs API
  slug: akta-pro-supporting-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akta-pro/refs/heads/main/openapi/akta-pro-supporting-apis-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: akta.pro
  spf: true
hosts:
- cert_expires: Nov 28 05:53:36 2026 GMT
  host: akta.pro
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Akta Pro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for akta.pro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: akta.pro
provider_slug: akta-pro
slug: akta-pro-domain-security
source_filename: akta-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: akta.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 05:53:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: akta.pro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akta-pro/refs/heads/main/security/akta-pro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Company Data
- Company Intelligence
- News
- Alternative Data
- Private Companies
- Firmographics
- Data Enrichment
- Signals
- MCP
- Market Intelligence
---
