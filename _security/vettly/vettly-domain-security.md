---
api_specs:
- filename: vettly-content-moderation-openapi.json
  format: json
  label: Vettly REST API
  slug: vettly-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vettly/refs/heads/main/openapi/vettly-content-moderation-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vettly.dev
  spf: false
hosts:
- cert_expires: Oct 16 09:00:12 2026 GMT
  host: docs.vettly.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 04:08:59 2026 GMT
  host: api.vettly.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Vettly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vettly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Vettly
provider_slug: vettly
slug: vettly-domain-security
source_filename: vettly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.vettly.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 09:00:12 2026 GMT\n  hsts: false\n- host: api.vettly.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 04:08:59 2026 GMT\n  hsts: null\ndomains:\n- domain: vettly.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vettly/refs/heads/main/security/vettly-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- content-moderation
- trust-and-safety
- security
- text-analysis
- image-moderation
- video-moderation
- UGC
- compliance
- agent-guardrails
- MCP
---
