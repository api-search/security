---
api_specs:
- filename: bright-data-access-api-openapi.yml
  format: yaml
  label: Bright Data Access API
  slug: bright-data-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-access-api-openapi.yml
- filename: bright-data-archive-api-openapi.yml
  format: yaml
  label: Bright Data Archive API
  slug: bright-data-archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-archive-api-openapi.yml
- filename: bright-data-billing-api-openapi.yml
  format: yaml
  label: Bright Data Billing API
  slug: bright-data-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-billing-api-openapi.yml
- filename: bright-data-datasets-api-openapi.yml
  format: yaml
  label: Bright Data Datasets API
  slug: bright-data-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-datasets-api-openapi.yml
- filename: bright-data-delivery-api-openapi.yml
  format: yaml
  label: Bright Data Delivery API
  slug: bright-data-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-delivery-api-openapi.yml
- filename: bright-data-ips-api-openapi.yml
  format: yaml
  label: Bright Data IPs API
  slug: bright-data-ips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-ips-api-openapi.yml
- filename: bright-data-lookup-api-openapi.yml
  format: yaml
  label: Bright Data Lookup API
  slug: bright-data-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-lookup-api-openapi.yml
- filename: bright-data-proxies-api-openapi.yml
  format: yaml
  label: Bright Data Proxies API
  slug: bright-data-proxies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-proxies-api-openapi.yml
- filename: bright-data-scrape-api-openapi.yml
  format: yaml
  label: Bright Data Scrape API
  slug: bright-data-scrape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-scrape-api-openapi.yml
- filename: bright-data-sessions-api-openapi.yml
  format: yaml
  label: Bright Data Sessions API
  slug: bright-data-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-sessions-api-openapi.yml
- filename: bright-data-shield-api-openapi.yml
  format: yaml
  label: Bright Data Shield API
  slug: bright-data-shield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-shield-api-openapi.yml
- filename: bright-data-snapshots-api-openapi.yml
  format: yaml
  label: Bright Data Snapshots API
  slug: bright-data-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-snapshots-api-openapi.yml
- filename: bright-data-tokens-api-openapi.yml
  format: yaml
  label: Bright Data Tokens API
  slug: bright-data-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-tokens-api-openapi.yml
- filename: bright-data-unlock-api-openapi.yml
  format: yaml
  label: Bright Data Unlock API
  slug: bright-data-unlock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-unlock-api-openapi.yml
- filename: bright-data-zones-api-openapi.yml
  format: yaml
  label: Bright Data Zones API
  slug: bright-data-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-zones-api-openapi.yml
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
