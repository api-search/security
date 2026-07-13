---
api_specs:
- filename: j-quants-openapi.yml
  format: yaml
  label: J-Quants API
  slug: j-quants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/j-quants/refs/heads/main/openapi/j-quants-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jpx-jquants.com
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: jquants.com
  spf: false
hosts:
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: jpx-jquants.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.jquants.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: J Quants Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for J-Quants, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: J-Quants
provider_slug: j-quants
slug: j-quants-domain-security
source_filename: j-quants-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jpx-jquants.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.jquants.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: jpx-jquants.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: jquants.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/j-quants/refs/heads/main/security/j-quants-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Data
- Investment
- Japan
- Stock Market
---
