---
api_specs:
- filename: scrapingbee-openapi.yml
  format: yaml
  label: ScrapingBee HTML API
  slug: html-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapingbee/refs/heads/main/openapi/scrapingbee-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scrapingbee.com
  spf: true
hosts:
- cert_expires: Sep 14 03:06:44 2026 GMT
  host: www.scrapingbee.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 08:10:19 2026 GMT
  host: app.scrapingbee.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scrapingbee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ScrapingBee, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ScrapingBee
provider_slug: scrapingbee
slug: scrapingbee-domain-security
source_filename: scrapingbee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scrapingbee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:06:44 2026 GMT\n  hsts: false\n- host: app.scrapingbee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 08:10:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: scrapingbee.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrapingbee/refs/heads/main/security/scrapingbee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Extraction
- Anti-Bot
- Data Aggregation
- Data Extraction
- Headless Browser
- JavaScript Rendering
- Proxy Rotation
- Screenshots
- Search Engine
- Web Scraping
---
