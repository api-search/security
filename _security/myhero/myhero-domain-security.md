---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tradehero.mobi
  spf: false
hosts:
- cert_expires: Oct 12 03:30:13 2026 GMT
  host: en.tradehero.mobi
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Myhero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Myhero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Myhero
provider_slug: myhero
slug: myhero-domain-security
source_filename: myhero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.tradehero.mobi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:30:13 2026 GMT\n  hsts: false\ndomains:\n- domain: tradehero.mobi\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/myhero/refs/heads/main/security/myhero-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fintech
- Trading
- Investing
- Stock Market
- Social Trading
- Mobile
- Gamification
- Singapore
---
