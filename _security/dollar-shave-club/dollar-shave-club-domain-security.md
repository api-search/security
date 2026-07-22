---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dollarshaveclub.com
  spf: true
hosts:
- cert_expires: Sep  9 12:00:02 2026 GMT
  host: www.dollarshaveclub.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dollar Shave Club Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dollar Shave Club, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dollar Shave Club
provider_slug: dollar-shave-club
slug: dollar-shave-club-domain-security
source_filename: dollar-shave-club-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dollarshaveclub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 12:00:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: dollarshaveclub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dollar-shave-club/refs/heads/main/security/dollar-shave-club-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- E-Commerce
- Subscription
- Direct-to-Consumer
- Retail
- Grooming
- Personal Care
---
