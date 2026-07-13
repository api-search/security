---
api_specs:
- filename: triplit-http-api-openapi.yml
  format: yaml
  label: Triplit HTTP API
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triplit/refs/heads/main/openapi/triplit-http-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: triplit.dev
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: triplit.io
  spf: false
hosts:
- host: www.triplit.dev
  https: false
- host: <project-id>.triplit.io
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''<project-id'
kind: domain-security
layout: security
method: probed
name: Triplit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Triplit, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Triplit
provider_slug: triplit
slug: triplit-domain-security
source_filename: triplit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.triplit.dev\n  https: false\n- host: <project-id>.triplit.io\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''<project-id'\n  hsts: null\ndomains:\n- domain: triplit.dev\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n- domain: triplit.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triplit/refs/heads/main/security/triplit-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Database
- Real-time
- Sync
- Local-first
- Developer Tools
- TypeScript
- Open Source
---
