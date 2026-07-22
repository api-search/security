---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: keno.ae
  spf: true
hosts:
- cert_expires: Nov 13 11:41:17 2026 GMT
  host: keno.ae
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Keno Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keno, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Keno
provider_slug: keno
slug: keno-domain-security
source_filename: keno-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keno.ae\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 13 11:41:17 2026 GMT\n  hsts: null\ndomains:\n- domain: keno.ae\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keno/refs/heads/main/security/keno-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Automotive
- Car Wash
- Vehicle Care
- Mobile App
- On-Demand
- Consumer
- UAE
---
