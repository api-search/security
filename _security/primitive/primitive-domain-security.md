---
api_specs:
- filename: primitive-openapi-original.json
  format: json
  label: Primitive API
  slug: primitive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: primitive.dev
  spf: true
hosts:
- cert_expires: Sep  1 21:19:35 2026 GMT
  host: www.primitive.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 21:13:20 2026 GMT
  host: api.primitive.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Primitive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Primitive, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Primitive
provider_slug: primitive
slug: primitive-domain-security
source_filename: primitive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.primitive.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 21:19:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.primitive.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 21:13:20 2026 GMT\n  hsts: null\ndomains:\n- domain: primitive.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/security/primitive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email
- Email Infrastructure
- AI Agents
- Agent Infrastructure
- Messaging
- Webhooks
- MCP
- Developer Tools
- API
---
