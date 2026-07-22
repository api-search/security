---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gyenno.com
  spf: true
hosts:
- cert_expires: Dec  8 09:26:25 2026 GMT
  host: gyenno.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Gyenno Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GYENNO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: GYENNO
provider_slug: gyenno
slug: gyenno-domain-security
source_filename: gyenno-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gyenno.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  8 09:26:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gyenno.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gyenno/refs/heads/main/security/gyenno-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Medical Devices
- Parkinson's Disease
- Assistive Technology
- Digital Health
- Wearables
- Neurology
- Consumer Health
---
