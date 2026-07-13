---
api_specs:
- filename: justcall-openapi.yml
  format: yaml
  label: JustCall REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justcall/refs/heads/main/openapi/justcall-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: justcall.io
  spf: true
hosts:
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: justcall.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 03:28:12 2026 GMT
  host: developer.justcall.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: api.justcall.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Justcall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JustCall, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: JustCall
provider_slug: justcall
slug: justcall-domain-security
source_filename: justcall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: justcall.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.justcall.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 03:28:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.justcall.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: justcall.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justcall/refs/heads/main/security/justcall-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Voice
- SMS
- Cloud Phone
- Contact Center
- Telephony
- Communications
---
