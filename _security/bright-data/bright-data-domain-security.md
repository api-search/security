---
api_specs:
- filename: bright-data-web-unlocker-api-openapi.yml
  format: yaml
  label: Bright Data Web Unlocker API
  slug: web-unlocker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-web-unlocker-api-openapi.yml
- filename: bright-data-serp-api-openapi.yml
  format: yaml
  label: Bright Data SERP API
  slug: serp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-serp-api-openapi.yml
- filename: bright-data-web-scraper-api-openapi.yml
  format: yaml
  label: Bright Data Web Scraper API
  slug: web-scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-web-scraper-api-openapi.yml
- filename: bright-data-scraping-browser-api-openapi.yml
  format: yaml
  label: Bright Data Scraping Browser API
  slug: scraping-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-scraping-browser-api-openapi.yml
- filename: bright-data-deep-lookup-api-openapi.yml
  format: yaml
  label: Bright Data Deep Lookup API
  slug: deep-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-deep-lookup-api-openapi.yml
- filename: bright-data-web-archive-api-openapi.yml
  format: yaml
  label: Bright Data Web Archive API
  slug: web-archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-web-archive-api-openapi.yml
- filename: bright-data-dataset-marketplace-api-openapi.yml
  format: yaml
  label: Bright Data Dataset Marketplace API
  slug: dataset-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-dataset-marketplace-api-openapi.yml
- filename: bright-data-account-management-api-openapi.yml
  format: yaml
  label: Bright Data Account Management API
  slug: account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-account-management-api-openapi.yml
- filename: bright-data-proxy-manager-api-openapi.yml
  format: yaml
  label: Bright Data Proxy Manager API
  slug: proxy-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-proxy-manager-api-openapi.yml
- filename: bright-data-scraping-shield-api-openapi.yml
  format: yaml
  label: Bright Data Scraping Shield API
  slug: scraping-shield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-scraping-shield-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brightdata.com
  spf: true
hosts:
- cert_expires: Sep 16 15:02:17 2026 GMT
  host: brightdata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 16:58:18 2026 GMT
  host: docs.brightdata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.brightdata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bright Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bright Data, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bright Data
provider_slug: bright-data
slug: bright-data-domain-security
source_filename: bright-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brightdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 15:02:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.brightdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 16:58:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.brightdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: brightdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/security/bright-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web Data
- Web Scraping
- Proxy
- Residential Proxy
- Datacenter Proxy
- ISP Proxy
- Mobile Proxy
- SERP
- Web Unlocker
- Scraping Browser
- Dataset Marketplace
- MCP
- AI Agents
---
