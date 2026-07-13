---
api_specs:
- filename: e2b-openapi.yml
  format: yaml
  label: E2B Sandbox API
  slug: sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b/refs/heads/main/openapi/e2b-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: e2b.dev
  spf: true
hosts:
- cert_expires: Aug 25 05:10:37 2026 GMT
  host: e2b.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 15:27:33 2026 GMT
  host: api.e2b.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: E2B Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for E2B, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: E2B
provider_slug: e2b
slug: e2b-domain-security
source_filename: e2b-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: e2b.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 05:10:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.e2b.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 15:27:33 2026 GMT\n  hsts: null\ndomains:\n- domain: e2b.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/e2b/refs/heads/main/security/e2b-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Code Interpreter
- Sandboxes
- Secure Execution
- AI Agents
- Firecracker
- microVMs
- Code Execution
- Data Analysis
- Desktop Sandbox
- Computer Use
- Custom Templates
- Python
- TypeScript
---
