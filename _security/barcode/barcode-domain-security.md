---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: barcodeapi.org
  spf: false
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: barcodeapi.org
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Barcode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BARCODE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: BARCODE
provider_slug: barcode
slug: barcode-domain-security
source_filename: barcode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: barcodeapi.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: barcodeapi.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barcode/refs/heads/main/security/barcode-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Barcodes
- Data
- Services
---
