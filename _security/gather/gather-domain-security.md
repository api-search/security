---
api_specs:
- filename: gather-http-api-openapi.yml
  format: yaml
  label: Gather HTTP API
  slug: gather-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gather/refs/heads/main/openapi/gather-http-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gather.town
  spf: true
hosts:
- cert_expires: Oct 14 00:06:36 2026 GMT
  host: gather.town
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gather Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gather, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gather
provider_slug: gather
slug: gather-domain-security
source_filename: gather-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gather.town\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 00:06:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gather.town\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gather/refs/heads/main/security/gather-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Future Of Work
- Virtual Office
- Video Conferencing
- Collaboration
- Metaverse
- Remote Work
- Events
---
