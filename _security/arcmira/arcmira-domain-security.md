---
api_specs:
- filename: arcmira-v1-openapi.json
  format: json
  label: Arcmira API V1 API
  slug: arcmira-api-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcmira/refs/heads/main/openapi/_original/arcmira-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arcmira.com
  spf: true
hosts:
- cert_expires: Dec 24 02:15:50 2026 GMT
  host: arcmira.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arcmira Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arcmira, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arcmira
provider_slug: arcmira
slug: arcmira-domain-security
source_filename: arcmira-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arcmira.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 02:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: arcmira.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcmira/refs/heads/main/security/arcmira-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Search
- YouTube
- Transcripts
- SDK
---
