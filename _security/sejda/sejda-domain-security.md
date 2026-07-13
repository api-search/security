---
api_specs:
- filename: sejda-openapi.yml
  format: yaml
  label: Sejda HTML to PDF API
  slug: sejda-html-to-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sejda/refs/heads/main/openapi/sejda-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sejda.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sejda.org
  spf: true
hosts:
- cert_expires: Oct  9 14:24:27 2026 GMT
  host: www.sejda.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 19:07:29 2026 GMT
  host: api.sejda.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 12:16:23 2026 GMT
  host: sejda.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sejda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sejda, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Sejda
provider_slug: sejda
slug: sejda-domain-security
source_filename: sejda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sejda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 14:24:27 2026 GMT\n  hsts: false\n- host: api.sejda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:07:29 2026 GMT\n  hsts: null\n- host: sejda.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 12:16:23 2026 GMT\n  hsts: false\ndomains:\n- domain: sejda.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: sejda.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sejda/refs/heads/main/security/sejda-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- PDF
- Document Conversion
- HTML to PDF
- PDF Editing
- OCR
---
