---
api_specs:
- filename: thordata-locations-api-openapi.yml
  format: yaml
  label: Thordata Locations API
  slug: thordata-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-locations-api-openapi.yml
- filename: thordata-proxy-extract-api-openapi.yml
  format: yaml
  label: Thordata Proxy IP Extract API
  slug: thordata-proxy-ip-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-proxy-extract-api-openapi.yml
- filename: thordata-account-api-openapi.yml
  format: yaml
  label: Thordata Account API
  slug: thordata-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-account-api-openapi.yml
- filename: thordata-proxy-api-openapi.yml
  format: yaml
  label: Thordata Proxy API
  slug: thordata-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-proxy-api-openapi.yml
- filename: thordata-proxy-users-api-openapi.yml
  format: yaml
  label: Thordata Proxy Users API
  slug: thordata-proxy-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-proxy-users-api-openapi.yml
- filename: thordata-serp-api-api-openapi.yml
  format: yaml
  label: Thordata SERP API
  slug: thordata-serp-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-serp-api-api-openapi.yml
- filename: thordata-tasks-api-openapi.yml
  format: yaml
  label: Thordata Tasks API
  slug: thordata-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-tasks-api-openapi.yml
- filename: thordata-universal-scraping-api-api-openapi.yml
  format: yaml
  label: Thordata Universal Scraping API
  slug: thordata-universal-scraping-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-universal-scraping-api-api-openapi.yml
- filename: thordata-web-scraper-api-api-openapi.yml
  format: yaml
  label: Thordata Web Scraper API
  slug: thordata-web-scraper-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-web-scraper-api-api-openapi.yml
- filename: thordata-whitelist-api-openapi.yml
  format: yaml
  label: Thordata Whitelist API
  slug: thordata-whitelist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-whitelist-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: thordata.com
  spf: true
hosts:
- cert_expires: Oct  2 08:16:55 2026 GMT
  host: doc.thordata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 19:36:28 2026 GMT
  host: scraperapi.thordata.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  1 19:36:28 2026 GMT
  host: openapi.thordata.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Thordata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thordata, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Thordata
provider_slug: thordata
slug: thordata-domain-security
source_filename: thordata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doc.thordata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 08:16:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: scraperapi.thordata.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 19:36:28 2026 GMT\n  hsts: null\n- host: openapi.thordata.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 19:36:28 2026 GMT\n  hsts: null\ndomains:\n- domain: thordata.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/security/thordata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Proxy network
- Web Scraping
- Data Extraction
- SERP
- Search data
- Web unblocking
- Residential Proxies
- Mobile Proxies
- ISP Proxies
- Datacenter Proxies
- Scraping Browser
- Data-for-AI
- RAG data pipelines
- Web Data
---
