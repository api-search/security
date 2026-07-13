---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: outscraper.com
  spf: true
hosts:
- cert_expires: Sep  3 05:21:58 2026 GMT
  host: app.outscraper.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 23:14:00 2026 GMT
  host: outscraper.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Outscraper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outscraper, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Outscraper
provider_slug: outscraper
slug: outscraper-domain-security
source_filename: outscraper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.outscraper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 05:21:58 2026 GMT\n  hsts: false\n- host: outscraper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 23:14:00 2026 GMT\n  hsts: false\ndomains:\n- domain: outscraper.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outscraper/refs/heads/main/security/outscraper-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Business Data
- Data Scraping
- Google Maps
---
