---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forex.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cityindex.com
  spf: true
hosts:
- cert_expires: Aug 14 19:42:06 2026 GMT
  host: www.forex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 00:15:21 2026 GMT
  host: ciapi.cityindex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Forex Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FOREX.com, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FOREX.com
provider_slug: forex-com
slug: forex-com-domain-security
source_filename: forex-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.forex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 19:42:06 2026 GMT\n  hsts: null\n- host: ciapi.cityindex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 00:15:21 2026 GMT\n  hsts: null\ndomains:\n- domain: forex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: cityindex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forex-com/refs/heads/main/security/forex-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Forex
- FX Trading
- CFD Trading
- Algorithmic Trading
- Financial Services
- Trading APIs
- Currency Exchange
---
