---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cheryinternational.com
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: chery.cn
  spf: false
hosts:
- cert_expires: Sep  1 23:59:59 2026 GMT
  host: www.cheryinternational.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: www.chery.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chery, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Chery
provider_slug: chery
slug: chery-domain-security
source_filename: chery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cheryinternational.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:59:59 2026 GMT\n  hsts: false\n- host: www.chery.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cheryinternational.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: chery.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chery/refs/heads/main/security/chery-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer Technology
- Automotive
- Automobile Manufacturer
- Electric Vehicles
- New Energy Vehicles
- China
- Connected Vehicles
---
