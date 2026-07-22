---
api_specs:
- filename: shapes-api-openapi.yml
  format: yaml
  label: Shapes API
  slug: shapes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapes/refs/heads/main/openapi/shapes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shapes.inc
  spf: true
hosts:
- cert_expires: Oct 19 00:26:05 2026 GMT
  host: shapes.inc
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: api.shapes.inc
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shapes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shapes, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Shapes
provider_slug: shapes
slug: shapes-domain-security
source_filename: shapes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shapes.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 00:26:05 2026 GMT\n  hsts: false\n- host: api.shapes.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: shapes.inc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shapes/refs/heads/main/security/shapes-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Chat
- Social
- Conversational AI
- LLM
- Voice
- Developer API
---
