---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: boaconsulta.com
  spf: true
hosts:
- cert_expires: Jan 10 01:40:01 2027 GMT
  host: www.boaconsulta.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boaconsulta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BoaConsulta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BoaConsulta
provider_slug: boaconsulta
slug: boaconsulta-domain-security
source_filename: boaconsulta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boaconsulta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 01:40:01 2027 GMT\n  hsts: null\ndomains:\n- domain: boaconsulta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boaconsulta/refs/heads/main/security/boaconsulta-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Telemedicine
- Appointment Booking
- Marketplace
- SaaS
- Practice Management
- Electronic Health Records
- Brazil
- LGPD
---
