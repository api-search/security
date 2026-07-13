---
api_specs:
- filename: openapi.json
  format: json
  label: PDFShift API
  slug: pdfshift-api
  spec_type: OpenAPI
  url: https://api.pdfshift.io/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pdfshift.io
  spf: true
hosts:
- cert_expires: Sep 15 01:21:03 2026 GMT
  host: pdfshift.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 06:43:22 2026 GMT
  host: docs.pdfshift.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 23:10:06 2026 GMT
  host: api.pdfshift.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pdfshift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PDFShift, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: PDFShift
provider_slug: pdfshift
slug: pdfshift-domain-security
source_filename: pdfshift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pdfshift.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:21:03 2026 GMT\n  hsts: false\n- host: docs.pdfshift.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 06:43:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.pdfshift.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 23:10:06 2026 GMT\n  hsts: false\ndomains:\n- domain: pdfshift.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pdfshift/refs/heads/main/security/pdfshift-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- PDF
- HTML to PDF
- Document Conversion
- Screenshot
- Chromium
- REST API
---
