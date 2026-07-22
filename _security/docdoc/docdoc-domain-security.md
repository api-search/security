---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: docdoc.com
  spf: true
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: docdoc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Docdoc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DocDoc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DocDoc
provider_slug: docdoc
slug: docdoc-domain-security
source_filename: docdoc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docdoc.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: docdoc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docdoc/refs/heads/main/security/docdoc-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Healthcare
- Health Technology
- Patient Empowerment
- Doctor Discovery
- Medical Advisory
- Asia
- Singapore
---
