---
api_specs:
- filename: openapi.yml
  format: yaml
  label: languagelayer API
  slug: languagelayer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/languagelayer/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: languagelayer.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apilayer.net
  spf: true
hosts:
- cert_expires: Oct  2 16:33:18 2026 GMT
  host: languagelayer.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: apilayer.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Languagelayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for languagelayer, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: languagelayer
provider_slug: languagelayer
slug: languagelayer-domain-security
source_filename: languagelayer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: languagelayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:33:18 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: apilayer.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: languagelayer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: apilayer.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/languagelayer/refs/heads/main/security/languagelayer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Language Detection
- Natural Language Processing
- Text Analysis
- Machine Learning
- AI
---
