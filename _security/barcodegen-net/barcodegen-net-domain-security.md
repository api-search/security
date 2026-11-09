---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: barcodegen.net
  spf: true
hosts:
- cert_expires: Jan 27 03:08:22 2027 GMT
  host: barcodegen.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Barcodegen Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Free Barcode Generator Online, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Free Barcode Generator Online
provider_slug: barcodegen-net
slug: barcodegen-net-domain-security
source_filename: barcodegen-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: barcodegen.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 03:08:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: barcodegen.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/barcodegen-net/security/barcodegen-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Barcodes
- Generator
- Free
- Online
---
