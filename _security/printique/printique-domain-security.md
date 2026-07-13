---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: printique.com
  spf: true
hosts:
- cert_expires: Jan 10 14:08:44 2027 GMT
  host: www.printique.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Printique Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Printique, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Printique
provider_slug: printique
slug: printique-domain-security
source_filename: printique-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.printique.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 10 14:08:44 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: printique.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/printique/refs/heads/main/security/printique-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Photo Printing
- Print Fulfillment
- Photo Lab
- Photography
- Prints
- Albums
- Wall Art
- Print on Demand
---
