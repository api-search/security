---
api_specs:
- filename: s1-dev-account-api-openapi.yml
  format: yaml
  label: Search1API Account API
  slug: s1-dev-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-account-api-openapi.yml
- filename: s1-dev-crawl-api-openapi.yml
  format: yaml
  label: Search1API Crawl API
  slug: s1-dev-crawl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-crawl-api-openapi.yml
- filename: s1-dev-feedback-api-openapi.yml
  format: yaml
  label: Search1API Feedback API
  slug: s1-dev-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-feedback-api-openapi.yml
- filename: s1-dev-screenshot-api-openapi.yml
  format: yaml
  label: Search1API Screenshot API
  slug: s1-dev-screenshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-screenshot-api-openapi.yml
- filename: s1-dev-search-api-openapi.yml
  format: yaml
  label: Search1API Search API
  slug: s1-dev-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-search-api-openapi.yml
- filename: s1-dev-system-api-openapi.yml
  format: yaml
  label: Search1API System API
  slug: s1-dev-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-system-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: s1.dev
  spf: false
hosts:
- cert_expires: Dec 17 12:40:20 2026 GMT
  host: s1.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: S1 Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Search1API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Search1API
provider_slug: s1-dev
slug: s1-dev-domain-security
source_filename: s1-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: s1.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 12:40:20 2026 GMT\n  hsts: false\ndomains:\n- domain: s1.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/security/s1-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Search
- Web Search
- Crawling
- Web Scraping
- News
- AI Agents
- MCP
- Agent Tools
- Data Extraction
- Screenshots
---
