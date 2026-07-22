---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jackpocket.com
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: jackpocket.com
  hsts: true
  hsts_max_age: 2628000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jackpocket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jackpocket, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jackpocket
provider_slug: jackpocket
slug: jackpocket-domain-security
source_filename: jackpocket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jackpocket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2628000\ndomains:\n- domain: jackpocket.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jackpocket/refs/heads/main/security/jackpocket-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Lottery
- Mobile App
- Consumer
- Fintech
---
