---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: js.org
  spf: true
hosts:
- cert_expires: Sep 29 14:27:59 2026 GMT
  host: cheerio.js.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cheerio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cheerio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cheerio
provider_slug: cheerio
slug: cheerio-domain-security
source_filename: cheerio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cheerio.js.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 14:27:59 2026 GMT\n  hsts: false\ndomains:\n- domain: js.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cheerio/refs/heads/main/security/cheerio-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Data Extraction
- DOM
- HTML
- HTML Parsing
- jQuery
- MIT License
- Node.js
- npm
- Open Source
- Parser
- Scraping
- Server-side
- Web Scraping
- XML
---
