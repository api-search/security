---
api_specs:
- filename: documenso-openapi.yml
  format: yaml
  label: Documenso Documents API
  slug: documents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/documenso/refs/heads/main/openapi/documenso-openapi.yml
- filename: documenso-openapi.yml
  format: yaml
  label: Documenso Recipients API
  slug: recipients
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/documenso/refs/heads/main/openapi/documenso-openapi.yml
- filename: documenso-openapi.yml
  format: yaml
  label: Documenso Fields API
  slug: fields
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/documenso/refs/heads/main/openapi/documenso-openapi.yml
- filename: documenso-openapi.yml
  format: yaml
  label: Documenso Templates API
  slug: templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/documenso/refs/heads/main/openapi/documenso-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: documenso.com
  spf: true
hosts:
- cert_expires: Oct  1 15:02:03 2026 GMT
  host: documenso.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 21:31:21 2026 GMT
  host: docs.documenso.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: app.documenso.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Documenso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Documenso, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Documenso
provider_slug: documenso
slug: documenso-domain-security
source_filename: documenso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: documenso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 15:02:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.documenso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 21:31:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.documenso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: documenso.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/documenso/refs/heads/main/security/documenso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Signature
- Documents
- Signing
- Open Source
- DocuSign Alternative
---
