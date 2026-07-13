---
api_specs:
- filename: crawlbase-openapi.yml
  format: yaml
  label: Crawlbase Crawling API
  slug: crawlbase-crawling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crawlbase/refs/heads/main/openapi/crawlbase-openapi.yml
- filename: crawlbase-openapi.yml
  format: yaml
  label: Crawlbase Scraper API
  slug: crawlbase-scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crawlbase/refs/heads/main/openapi/crawlbase-openapi.yml
- filename: crawlbase-openapi.yml
  format: yaml
  label: Crawlbase Cloud Storage API
  slug: crawlbase-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crawlbase/refs/heads/main/openapi/crawlbase-openapi.yml
- filename: crawlbase-openapi.yml
  format: yaml
  label: Crawlbase Screenshots API
  slug: crawlbase-screenshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crawlbase/refs/heads/main/openapi/crawlbase-openapi.yml
- filename: crawlbase-openapi.yml
  format: yaml
  label: Crawlbase Leads API
  slug: crawlbase-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crawlbase/refs/heads/main/openapi/crawlbase-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crawlbase.com
  spf: true
  spf_record: v=spf1 include:emsd1.com include:spf.zoho.com include:zoho.com include:em8389.crawlbase.com include:zeptomail.net mx -all
hosts:
- cert_expires: Aug 27 18:47:34 2026 GMT
  cert_not_before: May 29 17:51:33 2026 GMT
  host: crawlbase.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  server: cloudflare
  tls_version: TLSv1.3
- cert_expires: Oct 1 16:01:33 2026 GMT
  cert_not_before: Jul 3 16:01:34 2026 GMT
  host: api.crawlbase.com
  hsts: false
  https: true
  note: Returns HTTP 400 to an unauthenticated root request, as expected for the token-gated API host.
  server: PC-WS
kind: domain-security
layout: security
method: probed
name: Crawlbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crawlbase, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Crawlbase
provider_slug: crawlbase
slug: crawlbase-domain-security
source_filename: crawlbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crawlbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_not_before: May 29 17:51:33 2026 GMT\n  cert_expires: Aug 27 18:47:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  server: cloudflare\n- host: api.crawlbase.com\n  https: true\n  cert_not_before: Jul 3 16:01:34 2026 GMT\n  cert_expires: Oct 1 16:01:33 2026 GMT\n  hsts: false\n  server: PC-WS\n  note: Returns HTTP 400 to an unauthenticated root request, as expected for the token-gated API host.\ndomains:\n- domain: crawlbase.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:emsd1.com include:spf.zoho.com include:zoho.com include:em8389.crawlbase.com include:zeptomail.net mx -all\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crawlbase/refs/heads/main/security/crawlbase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web Scraping
- Web Crawling
- Web Intelligence
- Data Extraction
- Proxy
- Scraper API
- Data Collection
- SERP
- Web Data
---
