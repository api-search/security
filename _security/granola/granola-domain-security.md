---
api_specs:
- filename: granola-openapi.yml
  format: yaml
  label: Granola Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/granola/refs/heads/main/openapi/granola-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: granola.ai
  spf: true
hosts:
- cert_expires: Sep 16 06:37:51 2026 GMT
  host: www.granola.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 00:09:18 2026 GMT
  host: docs.granola.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: public-api.granola.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Granola Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Granola, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Granola
provider_slug: granola
slug: granola-domain-security
source_filename: granola-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.granola.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:37:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.granola.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 00:09:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: public-api.granola.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: granola.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/granola/refs/heads/main/security/granola-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Meeting Notes
- Transcription
- Productivity
- API
- MCP
- Zapier
- Business
- Enterprise
---
