---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: fancraze.com
  spf: true
hosts:
- cert_expires: Oct  5 03:56:25 2026 GMT
  host: www.fancraze.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fancraze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FanCraze, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: FanCraze
provider_slug: fancraze
slug: fancraze-domain-security
source_filename: fancraze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fancraze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 03:56:25 2026 GMT\n  hsts: false\ndomains:\n- domain: fancraze.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fancraze/refs/heads/main/security/fancraze-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Cricket
- Sports
- Collectibles
- Fantasy Sports
- Gaming
- Digital Collectibles
- Trading
---
