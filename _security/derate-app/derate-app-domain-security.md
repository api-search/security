---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: derate.app
  spf: false
hosts:
- cert_expires: Jan 18 18:57:06 2027 GMT
  host: derate.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Derate App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DERATE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: DERATE
provider_slug: derate-app
slug: derate-app-domain-security
source_filename: derate-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: derate.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 18:57:06 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: derate.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/derate-app/security/derate-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Truck
- Diagnostics
- Mobile App
- Automotive
- Spanish
---
