---
api_specs:
- filename: v0-platform-openapi.json
  format: json
  label: v0 Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v0/refs/heads/main/openapi/v0-platform-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: v0.app
  spf: false
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vercel.com
  spf: true
hosts:
- cert_expires: Aug 20 04:24:52 2026 GMT
  host: v0.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 08:55:49 2026 GMT
  host: vercel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 15:28:19 2026 GMT
  host: api.v0.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: V0 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for v0, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: v0
provider_slug: v0
slug: v0-domain-security
source_filename: v0-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: v0.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 04:24:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: vercel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 08:55:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.v0.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 15:28:19 2026 GMT\n  hsts: null\ndomains:\n- domain: v0.app\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n- domain: vercel.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/v0/refs/heads/main/security/v0-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- App Builder
- Vercel
- Code Generation
- Platform API
---
