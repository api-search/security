---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ipricegroup.com
  spf: true
hosts:
- cert_expires: Sep 30 11:44:03 2026 GMT
  host: ipricegroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iprice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iPrice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: iPrice
provider_slug: iprice
slug: iprice-domain-security
source_filename: iprice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ipricegroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 11:44:03 2026 GMT\n  hsts: false\ndomains:\n- domain: ipricegroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iprice/refs/heads/main/security/iprice-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- E-Commerce
- Price Comparison
- Southeast Asia
- Retail
- Coupons
- Shopping
- Aggregator
---
