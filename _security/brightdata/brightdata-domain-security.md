---
api_specs:
- filename: brightdata-openapi.yml
  format: yaml
  label: Bright Data Web Scraper API
  slug: brightdata-web-scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/openapi/brightdata-openapi.yml
- filename: brightdata-openapi.yml
  format: yaml
  label: Bright Data SERP API
  slug: brightdata-serp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/openapi/brightdata-openapi.yml
- filename: brightdata-openapi.yml
  format: yaml
  label: Bright Data Web Unlocker API
  slug: brightdata-web-unlocker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/openapi/brightdata-openapi.yml
- filename: brightdata-openapi.yml
  format: yaml
  label: Bright Data Proxy & Zone Management API
  slug: brightdata-proxy-zone-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/openapi/brightdata-openapi.yml
- filename: brightdata-openapi.yml
  format: yaml
  label: Bright Data Datasets API
  slug: brightdata-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/openapi/brightdata-openapi.yml
- filename: brightdata-openapi.yml
  format: yaml
  label: Bright Data Browser API (Scraping Browser)
  slug: brightdata-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/openapi/brightdata-openapi.yml
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
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.brightdata.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 16:58:18 2026 GMT
  host: docs.brightdata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brightdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bright Data, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bright Data
provider_slug: brightdata
slug: brightdata-domain-security
source_filename: brightdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brightdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 15:02:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n- host: api.brightdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: docs.brightdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 16:58:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: brightdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/security/brightdata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web Data
- Web Scraping
- Web Intelligence
- Proxy
- Data Extraction
- SERP
- Web Unlocker
- Datasets
- Data Collection
- Browser Automation
---
