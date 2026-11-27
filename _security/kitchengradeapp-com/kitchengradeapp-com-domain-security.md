---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kitchengradeapp.com
  spf: false
hosts:
- cert_expires: Jan  5 13:43:46 2027 GMT
  host: kitchengradeapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: KitchenGrade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KitchenGrade, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: KitchenGrade
provider_slug: kitchengradeapp-com
slug: kitchengradeapp-com-domain-security
source_filename: kitchengradeapp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kitchengradeapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 13:43:46 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kitchengradeapp.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kitchengradeapp-com/security/kitchengradeapp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Data
- Restaurant
- Inspection
- Florida
- Public APIs
---
