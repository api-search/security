---
api_specs:
- filename: beyond-presence-openapi-original.json
  format: json
  label: Beyond Presence API
  slug: beyond-presence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-presence/refs/heads/main/openapi/beyond-presence-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bey.dev
  spf: true
hosts:
- cert_expires: Aug 26 00:20:38 2026 GMT
  host: api.bey.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beyond Presence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beyond Presence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Beyond Presence
provider_slug: beyond-presence
slug: beyond-presence-domain-security
source_filename: beyond-presence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.bey.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 00:20:38 2026 GMT\n  hsts: null\ndomains:\n- domain: bey.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beyond-presence/refs/heads/main/security/beyond-presence-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Ai Enterprise Software
- Artificial Intelligence
- Avatars
- Video
- Conversational AI
- Agents
- Speech To Video
- Real Time Communication
---
