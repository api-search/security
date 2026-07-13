---
api_specs:
- filename: spider-cloud-openapi.yml
  format: yaml
  label: Spider API
  slug: spider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spider-cloud/refs/heads/main/openapi/spider-cloud-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spider.cloud
  spf: false
hosts:
- cert_expires: Oct  5 02:28:54 2026 GMT
  host: spider.cloud
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api.spider.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: mcp.spider.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spider Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spider, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Spider
provider_slug: spider-cloud
slug: spider-cloud-domain-security
source_filename: spider-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spider.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 02:28:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.spider.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: false\n- host: mcp.spider.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: spider.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spider-cloud/refs/heads/main/security/spider-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Crawling
- Scraping
- Data Extraction
- URLs
- AI
- Markdown
- MCP
- Rust
- Headless Browser
- Proxies
---
