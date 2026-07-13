---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: scrapy.org
  spf: true
hosts:
- cert_expires: Aug 16 08:50:00 2026 GMT
  host: scrapy.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scrapy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scrapy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Scrapy
provider_slug: scrapy
slug: scrapy-domain-security
source_filename: scrapy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scrapy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 08:50:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: scrapy.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrapy/refs/heads/main/security/scrapy-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Crawling
- Data Extraction
- Scraping
---
