---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hodl.mobi
  spf: true
hosts:
- cert_expires: Aug 30 08:22:26 2026 GMT
  host: hodl.mobi
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hodl Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HODL Media, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HODL Media
provider_slug: hodl-media
slug: hodl-media-domain-security
source_filename: hodl-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hodl.mobi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:22:26 2026 GMT\n  hsts: false\ndomains:\n- domain: hodl.mobi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hodl-media/refs/heads/main/security/hodl-media-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cryptocurrency
- Stocks
- Market Data
- Portfolio Tracking
- Mobile App
- Finance
---
