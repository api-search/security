---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: worldfirst.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: worldfirst.com.cn
  spf: true
hosts:
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: www.worldfirst.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: developers.worldfirst.com.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar 14 23:59:59 2027 GMT
  host: open-sea.worldfirst.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Worldfirst Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WorldFirst, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WorldFirst
provider_slug: worldfirst
slug: worldfirst-domain-security
source_filename: worldfirst-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.worldfirst.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developers.worldfirst.com.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: false\n- host: open-sea.worldfirst.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: worldfirst.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: worldfirst.com.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worldfirst/refs/heads/main/security/worldfirst-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- United Kingdom
- Cross-Border
- Money Transfer
- Foreign Exchange
- Payouts
- Payment Gateway
- E-commerce
- Multi-Currency
- Card Issuing
---
