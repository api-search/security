---
api_specs:
- filename: pdfbroker-io-pdf-api-openapi.yml
  format: yaml
  label: pdfbroker-io PDF API
  slug: pdfbroker-io-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfbroker-io/openapi/pdfbroker-io-pdf-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pdfbroker.io
  spf: true
hosts:
- cert_expires: Apr  1 23:59:59 2027 GMT
  host: pdfbroker.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pdfbroker Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pdfbroker-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: pdfbroker-io
provider_slug: pdfbroker-io
slug: pdfbroker-io-domain-security
source_filename: pdfbroker-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pdfbroker.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: pdfbroker.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/pdfbroker-io/security/pdfbroker-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- PDF Generation
- REST API
- HTML to PDF
- PDF/A
- PDF/UA
- PDF Utilities
- XSL-FO
---
