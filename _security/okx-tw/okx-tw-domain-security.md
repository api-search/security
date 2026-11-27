---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: okx.tw
  spf: true
hosts:
- cert_expires: Feb  6 09:14:24 2027 GMT
  host: okx.tw
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CHAOS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CHAOS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CHAOS
provider_slug: okx-tw
slug: okx-tw-domain-security
source_filename: okx-tw-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: okx.tw\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 09:14:24 2027 GMT\n  hsts: false\ndomains:\n- domain: okx.tw\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/okx-tw/security/okx-tw-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Analytics
- Cryptocurrency
- Trading
- Market Data
---
