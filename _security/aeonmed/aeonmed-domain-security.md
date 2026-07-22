---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aeonmed.com
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: www.aeonmed.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Aeonmed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aeonmed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: aeonmed
provider_slug: aeonmed
slug: aeonmed-domain-security
source_filename: aeonmed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aeonmed.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aeonmed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeonmed/refs/heads/main/security/aeonmed-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Medical Devices
- Healthcare
- Anesthesia
- Ventilators
- Respiratory
- Medical Equipment
- Operating Room
- Intensive Care
---
