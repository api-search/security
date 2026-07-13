---
api_specs:
- filename: lingo-dev-openapi.yml
  format: yaml
  label: Lingo.dev Engine API (Localize)
  slug: engine-api-localize
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lingo-dev/refs/heads/main/openapi/lingo-dev-openapi.yml
- filename: lingo-dev-openapi.yml
  format: yaml
  label: Lingo.dev SDK
  slug: sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lingo-dev/refs/heads/main/openapi/lingo-dev-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lingo.dev
  spf: true
hosts:
- cert_expires: Oct  8 22:29:05 2026 GMT
  host: lingo.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 04:58:43 2026 GMT
  host: api.lingo.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lingo Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lingo.dev, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Lingo.dev
provider_slug: lingo-dev
slug: lingo-dev-domain-security
source_filename: lingo-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lingo.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 22:29:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lingo.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 04:58:43 2026 GMT\n  hsts: null\ndomains:\n- domain: lingo.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lingo-dev/refs/heads/main/security/lingo-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Localization
- Translation
- i18n
- Developer Tools
---
