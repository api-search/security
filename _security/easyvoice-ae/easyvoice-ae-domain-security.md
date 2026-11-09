---
api_specs:
- filename: easyvoice-ae-openapi-generated.yml
  format: yaml
  label: EasyVoice API
  slug: easyvoice-ae-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easyvoice-ae/openapi/_ae-authored/easyvoice-ae-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: easyvoice.ae
  spf: false
hosts:
- cert_expires: Dec 23 19:11:12 2026 GMT
  host: easyvoice.ae
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Easyvoice Ae Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EasyVoice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: EasyVoice
provider_slug: easyvoice-ae
slug: easyvoice-ae-domain-security
source_filename: easyvoice-ae-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: easyvoice.ae\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 19:11:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: easyvoice.ae\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/easyvoice-ae/security/easyvoice-ae-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Text-to-Speech
- Artificial Intelligence
- Voice
- United Arab Emirates
---
