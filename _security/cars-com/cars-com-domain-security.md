---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cars.com
  spf: true
hosts:
- cert_expires: May 13 23:59:59 2027 GMT
  host: cars.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cars.com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cars.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cars.com
provider_slug: cars-com
slug: cars-com-domain-security
source_filename: cars-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cars.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cars.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cars-com/security/cars-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Car Buying
- Car Selling
- Vehicle Research
---
