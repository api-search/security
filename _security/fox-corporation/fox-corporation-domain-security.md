---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: foxcorporation.com
  spf: true
hosts:
- cert_expires: Sep  5 23:59:59 2026 GMT
  host: www.foxcorporation.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fox Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fox Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fox Corporation
provider_slug: fox-corporation
slug: fox-corporation-domain-security
source_filename: fox-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.foxcorporation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: foxcorporation.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fox-corporation/refs/heads/main/security/fox-corporation-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Media
- Broadcasting
- News
- Sports
- Entertainment
- Streaming
- Television
- Free Ad-Supported Streaming
- Sports Betting
- Fortune 500
---
