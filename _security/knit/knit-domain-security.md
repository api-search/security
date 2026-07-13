---
api_specs:
- filename: knit-unified-api-openapi.yml
  format: yaml
  label: Knit Unified API
  slug: unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knit/refs/heads/main/openapi/knit-unified-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getknit.dev
  spf: true
hosts:
- cert_expires: Oct  4 22:11:15 2026 GMT
  host: developers.getknit.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: api.getknit.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Knit
provider_slug: knit
slug: knit-domain-security
source_filename: knit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.getknit.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:11:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getknit.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: getknit.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knit/refs/heads/main/security/knit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- HR Integrations
- HRIS
- Unified API
---
