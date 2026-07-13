---
api_specs:
- filename: dead-drop-openapi.yml
  format: yaml
  label: Dead Drop API v1
  slug: dead-drop-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dead-drop/refs/heads/main/openapi/dead-drop-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dead-drop.xyz
  spf: false
hosts:
- cert_expires: Aug 14 02:29:00 2026 GMT
  host: dead-drop.xyz
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 17:57:35 2026 GMT
  host: api.dead-drop.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dead Drop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dead Drop, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Dead Drop
provider_slug: dead-drop
slug: dead-drop-domain-security
source_filename: dead-drop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dead-drop.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 02:29:00 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: api.dead-drop.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 17:57:35 2026 GMT\n  hsts: null\ndomains:\n- domain: dead-drop.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dead-drop/refs/heads/main/security/dead-drop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Messaging
- Privacy
- Anonymous
- Open Source
---
