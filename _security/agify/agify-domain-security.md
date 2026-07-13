---
api_specs:
- filename: agify-openapi.json
  format: json
  label: Agify Age Prediction API
  slug: agify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agify/refs/heads/main/openapi/agify-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: agify.io
  spf: false
hosts:
- cert_expires: Sep 27 14:12:54 2026 GMT
  host: agify.io
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 27 14:12:54 2026 GMT
  host: api.agify.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Agify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agify.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Agify.io
provider_slug: agify
slug: agify-domain-security
source_filename: agify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agify.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 14:12:54 2026 GMT\n  hsts: false\n- host: api.agify.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 14:12:54 2026 GMT\n  hsts: null\ndomains:\n- domain: agify.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agify/refs/heads/main/security/agify-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Age Prediction
- Name Analysis
- Demographics
- Statistical API
- Free API
---
