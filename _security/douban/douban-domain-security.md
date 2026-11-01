---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: douban.com
  spf: true
hosts:
- cert_expires: Dec 27 03:54:07 2026 GMT
  host: douban.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Douban Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Douban, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Douban
provider_slug: douban
slug: douban-domain-security
source_filename: douban-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: douban.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 03:54:07 2026 GMT\n  hsts: null\ndomains:\n- domain: douban.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/douban/security/douban-domain-security.yml
summary_line: TLSv1.2
tags:
- Social
- Media
- Entertainment
- China
- API
---
