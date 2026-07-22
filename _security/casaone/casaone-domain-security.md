---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: casaone.com
  spf: false
hosts:
- cert_expires: Sep 11 23:31:34 2026 GMT
  host: www.casaone.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Casaone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CasaOne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CasaOne
provider_slug: casaone
slug: casaone-domain-security
source_filename: casaone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.casaone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:31:34 2026 GMT\n  hsts: null\ndomains:\n- domain: casaone.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/casaone/refs/heads/main/security/casaone-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer
- Furniture
- Rental
- Home
- E-commerce
- Staging
- Interior Design
---
