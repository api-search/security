---
api_specs:
- filename: escape-openapi.yml
  format: yaml
  label: Escape Public API
  slug: escape-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: escape.tech
  spf: true
hosts:
- cert_expires: Aug 31 20:25:53 2026 GMT
  host: escape.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  9 13:30:49 2026 GMT
  host: docs.escape.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: public.escape.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Escape Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Escape, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Escape
provider_slug: escape
slug: escape-domain-security
source_filename: escape-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: escape.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 20:25:53 2026 GMT\n  hsts: false\n- host: docs.escape.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 13:30:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: public.escape.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: escape.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/security/escape-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Platform
- Security
---
