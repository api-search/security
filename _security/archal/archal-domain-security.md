---
api_specs:
- filename: archal-openapi-original.json
  format: json
  label: Archal API
  slug: archal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archal/refs/heads/main/openapi/archal-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: archal.ai
  spf: true
hosts:
- cert_expires: Sep 19 04:04:30 2026 GMT
  host: archal.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.archal.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Archal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Archal, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Archal
provider_slug: archal
slug: archal-domain-security
source_filename: archal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: archal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 04:04:30 2026 GMT\n  hsts: null\n- host: api.archal.ai\n  https: false\ndomains:\n- domain: archal.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archal/refs/heads/main/security/archal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI Agents
- Agent Testing
- Developer Tools
- API Testing
- Sandbox
- Evaluation
- Infrastructure
---
