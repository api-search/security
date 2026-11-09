---
api_specs:
- filename: docmorph-dev-tools-api-openapi.yml
  format: yaml
  label: DocMorph Tools API
  slug: docmorph-dev-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docmorph-dev/openapi/docmorph-dev-tools-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: docmorph.dev
  spf: true
hosts:
- cert_expires: Jan  1 12:46:39 2027 GMT
  host: docmorph.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Docmorph Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DocMorph, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DocMorph
provider_slug: docmorph-dev
slug: docmorph-dev-domain-security
source_filename: docmorph-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docmorph.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 12:46:39 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: docmorph.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/docmorph-dev/security/docmorph-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Document Processing
- Privacy
- OCR
- Media
- Local-First
---
