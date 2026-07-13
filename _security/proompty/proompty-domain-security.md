---
api_specs:
- filename: proompty-openapi-original.yml
  format: yaml
  label: Proompty
  slug: proompty
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/proompty/refs/heads/main/openapi/proompty-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: proompty.com
  spf: true
hosts:
- cert_expires: Aug 22 02:40:06 2026 GMT
  host: app.proompty.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Proompty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Proompty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Proompty
provider_slug: proompty
slug: proompty-domain-security
source_filename: proompty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.proompty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 02:40:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: proompty.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proompty/refs/heads/main/security/proompty-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Prompts
---
