---
api_specs:
- filename: eagle-doc-doc-api-openapi.yml
  format: yaml
  label: Eagle Doc API
  slug: eagle-doc-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eagle-doc/openapi/eagle-doc-doc-api-openapi.yml
- filename: eagle-doc-openapi-generated.yml
  format: yaml
  label: Eagle Doc API
  slug: eagle-doc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eagle-doc/openapi/_ae-authored/eagle-doc-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eagle-doc.com
  spf: true
hosts:
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: eagle-doc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eagle Doc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eagle Doc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Eagle Doc
provider_slug: eagle-doc
slug: eagle-doc-domain-security
source_filename: eagle-doc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eagle-doc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: eagle-doc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/eagle-doc/security/eagle-doc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- OCR
- Bookkeeping
- Document-Processing
- API
---
