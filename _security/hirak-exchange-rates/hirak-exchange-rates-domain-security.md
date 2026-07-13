---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hirak.site
  spf: false
hosts:
- cert_expires: Sep 23 01:30:27 2026 GMT
  host: rates.hirak.site
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hirak Exchange Rates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hirak Exchange Rates, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Hirak Exchange Rates
provider_slug: hirak-exchange-rates
slug: hirak-exchange-rates-domain-security
source_filename: hirak-exchange-rates-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rates.hirak.site\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 01:30:27 2026 GMT\n  hsts: null\ndomains:\n- domain: hirak.site\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hirak-exchange-rates/refs/heads/main/security/hirak-exchange-rates-domain-security.yml
summary_line: TLSv1.3
tags:
- Cryptocurrency
- Public APIs
---
