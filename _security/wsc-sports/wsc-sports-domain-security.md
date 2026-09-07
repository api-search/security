---
api_specs:
- filename: wsc-sports-blaze-feed-api.json
  format: json
  label: WSC Sports Blaze Feed API
  slug: wsc-sports-blaze-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wsc-sports/refs/heads/main/openapi/wsc-sports-blaze-feed-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wsc-sports.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: clipro.tv
  spf: false
hosts:
- cert_expires: Nov 26 10:54:37 2026 GMT
  host: wsc-sports.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 00:01:54 2026 GMT
  host: dev.wsc-sports.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: blazefeed.clipro.tv
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Wsc Sports Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WSC Sports, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: WSC Sports
provider_slug: wsc-sports
slug: wsc-sports-domain-security
source_filename: wsc-sports-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wsc-sports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 10:54:37 2026 GMT\n  hsts: false\n- host: dev.wsc-sports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 00:01:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: blazefeed.clipro.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: wsc-sports.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: clipro.tv\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wsc-sports/refs/heads/main/security/wsc-sports-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sports
- Video
- Media
- Artificial Intelligence
- Content
- Streaming
- SDK
- Highlights
- Personalization
---
