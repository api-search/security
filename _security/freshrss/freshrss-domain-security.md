---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: freshrss.org
  spf: true
hosts:
- cert_expires: Dec  1 03:22:10 2026 GMT
  host: freshrss.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Freshrss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreshRSS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: FreshRSS
provider_slug: freshrss
slug: freshrss-domain-security
source_filename: freshrss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freshrss.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  1 03:22:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: freshrss.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/freshrss/security/freshrss-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC
tags:
- RSS Aggregator
- Self‑Hosted Software
- Feed Reader
- Web Scraping
- OPML
- WebSub
- Open Source
---
