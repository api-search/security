---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: adcolony.com
  spf: true
hosts:
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: www.adcolony.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adcolony Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdColony, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: AdColony
provider_slug: adcolony
slug: adcolony-domain-security
source_filename: adcolony-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adcolony.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: adcolony.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adcolony/refs/heads/main/security/adcolony-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Mobile Advertising
- AdTech
- SDK
- Monetization
- Mobile
---
