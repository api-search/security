---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fanfest.vip
  spf: false
hosts:
- cert_expires: Oct 15 05:33:57 2026 GMT
  host: fanfest.vip
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vici Sports Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VICI Sports, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: VICI Sports
provider_slug: vici-sports
slug: vici-sports-domain-security
source_filename: vici-sports-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fanfest.vip\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 05:33:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fanfest.vip\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vici-sports/refs/heads/main/security/vici-sports-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sports
- Fan Engagement
- Sports Technology
- Marketing
- Loyalty
---
