---
api_specs:
- filename: narrador-io-account-api-openapi.yml
  format: yaml
  label: Narrador Account API
  slug: narrador-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/narrador-io/openapi/narrador-io-account-api-openapi.yml
- filename: narrador-io-narrador-files-api-openapi.yml
  format: yaml
  label: Narrador narrador files API
  slug: narrador-io-narrador-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/narrador-io/openapi/narrador-io-narrador-files-api-openapi.yml
- filename: narrador-io-narrador-x-api-openapi.yml
  format: yaml
  label: Narrador narrador X API
  slug: narrador-io-narrador-x-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/narrador-io/openapi/narrador-io-narrador-x-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: narrador.io
  spf: true
hosts:
- cert_expires: Jan  4 18:16:04 2027 GMT
  host: narrador.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Narrador Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Narrador, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Narrador
provider_slug: narrador-io
slug: narrador-io-domain-security
source_filename: narrador-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: narrador.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 18:16:04 2027 GMT\n  hsts: false\ndomains:\n- domain: narrador.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/narrador-io/security/narrador-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Text-to-Speech
- Audio
- Video
- Document Conversion
- X Posts
---
