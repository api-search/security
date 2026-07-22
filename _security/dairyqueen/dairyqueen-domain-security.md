---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dairyqueen.com
  spf: true
hosts:
- cert_expires: Sep 13 19:10:50 2026 GMT
  host: dairyqueen.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dairyqueen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dairyqueen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dairyqueen
provider_slug: dairyqueen
slug: dairyqueen-domain-security
source_filename: dairyqueen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dairyqueen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 19:10:50 2026 GMT\n  hsts: null\ndomains:\n- domain: dairyqueen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dairyqueen/refs/heads/main/security/dairyqueen-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Restaurant
- Fast Food
- Ice Cream
- Quick Service Restaurant
- Franchise
- Food and Beverage
- Consumer
---
