---
api_specs:
- filename: scraper-api-openapi.yml
  format: yaml
  label: ScraperAPI
  slug: scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scraper-api/refs/heads/main/openapi/scraper-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: scraperapi.com
  spf: true
hosts:
- cert_expires: Oct  2 04:07:49 2026 GMT
  host: www.scraperapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 28 00:42:41 2026 GMT
  host: api.scraperapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 14:50:23 2026 GMT
  host: async.scraperapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scraper Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ScraperAPI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ScraperAPI
provider_slug: scraper-api
slug: scraper-api-domain-security
source_filename: scraper-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scraperapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 04:07:49 2026 GMT\n  hsts: false\n- host: api.scraperapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 00:42:41 2026 GMT\n  hsts: null\n- host: async.scraperapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 14:50:23 2026 GMT\n  hsts: null\ndomains:\n- domain: scraperapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scraper-api/refs/heads/main/security/scraper-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data Extraction
- Proxies
- Scraping
---
