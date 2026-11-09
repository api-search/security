---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coinfuty.com
  spf: false
hosts:
- cert_expires: Jan  8 11:25:41 2027 GMT
  host: coinfuty.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coinfuty Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coinfuty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Coinfuty
provider_slug: coinfuty-com
slug: coinfuty-com-domain-security
source_filename: coinfuty-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coinfuty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 11:25:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: coinfuty.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/coinfuty-com/security/coinfuty-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Crypto Futures
- Market Data
- Open Interest
- Funding Rates
- Liquidations
- Indicators
---
