---
api_specs:
- filename: amazon-scraper-api-openapi-original.json
  format: json
  label: Amazon Scraper REST API
  slug: amazon-scraper-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-scraper-api/refs/heads/main/openapi/amazon-scraper-api-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amazonscraperapi.com
  spf: true
hosts:
- cert_expires: Nov 30 04:45:19 2026 GMT
  host: amazonscraperapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 18:31:22 2026 GMT
  host: api.amazonscraperapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Amazon Scraper Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Scraper API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amazon Scraper API
provider_slug: amazon-scraper-api
slug: amazon-scraper-api-domain-security
source_filename: amazon-scraper-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amazonscraperapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 04:45:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.amazonscraperapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 18:31:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: amazonscraperapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-scraper-api/refs/heads/main/security/amazon-scraper-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web Scraping
- Data Extraction
- E-Commerce Data
- Amazon
- marketplace data
- Product Intelligence
- Price Monitoring
- Competitor Research
- MCP
- Agent Tooling
---
