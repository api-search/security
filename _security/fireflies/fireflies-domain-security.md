---
api_specs:
- filename: openapi.json
  format: json
  label: Fireflies GraphQL API
  slug: fireflies-graphql-api
  spec_type: OpenAPI
  url: https://docs.fireflies.ai/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fireflies.ai
  spf: true
hosts:
- cert_expires: Sep 27 00:04:16 2026 GMT
  host: fireflies.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 13:20:39 2026 GMT
  host: docs.fireflies.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 00:04:16 2026 GMT
  host: api.fireflies.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fireflies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fireflies.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fireflies.ai
provider_slug: fireflies
slug: fireflies-domain-security
source_filename: fireflies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fireflies.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 00:04:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.fireflies.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 13:20:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.fireflies.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 00:04:16 2026 GMT\n  hsts: null\ndomains:\n- domain: fireflies.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fireflies/refs/heads/main/security/fireflies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Meeting Assistant
- Transcription
- Summaries
- Action Items
- GraphQL
- Meetings
- Productivity
- Collaboration
- Conversation Intelligence
---
