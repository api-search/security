---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dkmedtech.com
  spf: true
hosts:
- cert_expires: Oct 11 15:59:59 2026 GMT
  host: dkmedtech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dkmedtech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dkmedtech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: dkmedtech
provider_slug: dkmedtech
slug: dkmedtech-domain-security
source_filename: dkmedtech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dkmedtech.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 11 15:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dkmedtech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dkmedtech/refs/heads/main/security/dkmedtech-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Medical Devices
- MedTech
- Healthcare
- Cardiovascular
- Interventional Devices
- China
---
