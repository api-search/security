---
api_specs:
- filename: docs.pdffiller.com
  format: yaml
  label: PDFfiller REST API
  slug: pdffiller-api
  spec_type: OpenAPI
  url: https://docs.pdffiller.com
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pdffiller.com
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: www.pdffiller.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 19:48:38 2026 GMT
  host: docs.pdffiller.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: api.pdffiller.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pdffiller Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PDFfiller, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PDFfiller
provider_slug: pdffiller
slug: pdffiller-domain-security
source_filename: pdffiller-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pdffiller.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pdffiller.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 19:48:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pdffiller.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: pdffiller.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pdffiller/refs/heads/main/security/pdffiller-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- PDF
- E-Signature
- Document Management
- Form Builder
- PDF Editing
- Electronic Signature
- Document Workflow
---
