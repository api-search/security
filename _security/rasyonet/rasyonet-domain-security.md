---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rasyonet.com.tr
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rasyonet.com
  spf: true
hosts:
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: www.rasyonet.com.tr
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: www.rasyonet.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rasyonet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rasyonet, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Rasyonet
provider_slug: rasyonet
slug: rasyonet-domain-security
source_filename: rasyonet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rasyonet.com.tr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\n- host: www.rasyonet.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: rasyonet.com.tr\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: rasyonet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rasyonet/refs/heads/main/security/rasyonet-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Capital Markets
- E-Commerce
- Equity Research
- Financial Data
- Financial Services
- Fintech
- Grocery
- Investment Management
- Portfolio Analytics
- Retail
- Turkey
---
