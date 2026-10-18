---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: excelpricefeed.com
  spf: false
hosts:
- cert_expires: Dec 15 07:18:05 2026 GMT
  host: excelpricefeed.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Excelpricefeed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Excel Price Feed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Excel Price Feed
provider_slug: excelpricefeed
slug: excelpricefeed-domain-security
source_filename: excelpricefeed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: excelpricefeed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 07:18:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: excelpricefeed.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/excelpricefeed/refs/heads/main/security/excelpricefeed-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Finance
- Excel
- Real-Time Data
---
