---
api_specs:
- filename: lilt-openapi-original.yml
  format: yaml
  label: LILT API
  slug: lilt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lilt.com
  spf: true
hosts:
- cert_expires: Oct 11 00:29:47 2026 GMT
  host: lilt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 11:26:37 2026 GMT
  host: support.lilt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 17:19:34 2026 GMT
  host: api.lilt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lilt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lilt, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lilt
provider_slug: lilt
slug: lilt-domain-security
source_filename: lilt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lilt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 00:29:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: support.lilt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 11:26:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.lilt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 17:19:34 2026 GMT\n  hsts: null\ndomains:\n- domain: lilt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/security/lilt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Translation
- Localization
- Machine Translation
- Language
- Content
- Translation Memory
- Agents
---
