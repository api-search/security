---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: huntprice.ca
  spf: true
hosts:
- cert_expires: Jan  8 11:13:40 2027 GMT
  host: huntprice.ca
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HuntPrice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HuntPrice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HuntPrice
provider_slug: huntprice-ca
slug: huntprice-ca-domain-security
source_filename: huntprice-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: huntprice.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 11:13:40 2027 GMT\n  hsts: null\ndomains:\n- domain: huntprice.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/huntprice-ca/security/huntprice-ca-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Grocery
- Price Comparison
- Canada
- OpenAPI
---
