---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dewu.com
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: dewu.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dewu Poizon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dewu (POIZON), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dewu (POIZON)
provider_slug: dewu-poizon
slug: dewu-poizon-domain-security
source_filename: dewu-poizon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dewu.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: dewu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dewu-poizon/refs/heads/main/security/dewu-poizon-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Technology
- E-Commerce
- Marketplace
- Retail
- Sneakers
- Luxury Goods
- Authentication
- China
---
