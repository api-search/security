---
api_specs:
- filename: reqres-openapi.yml
  format: yaml
  label: ReqRes API
  slug: reqres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reqres/refs/heads/main/openapi/reqres-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reqres.in
  spf: true
hosts:
- cert_expires: Oct  9 12:11:58 2026 GMT
  host: reqres.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reqres Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReqRes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ReqRes
provider_slug: reqres
slug: reqres-domain-security
source_filename: reqres-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reqres.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 12:11:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reqres.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reqres/refs/heads/main/security/reqres-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Development
- Testing
- Prototyping
- Fake API
- REST
- Agent Sandbox
---
