---
api_specs:
- filename: e2b-api-openapi.yml
  format: yaml
  label: E2B Sandbox API
  slug: e2b-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-api-openapi.yml
- filename: e2b-api-openapi.yml
  format: yaml
  label: E2B Template API
  slug: e2b-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-api-openapi.yml
- filename: e2b-api-openapi.yml
  format: yaml
  label: E2B Volume API
  slug: e2b-volume-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-api-openapi.yml
- filename: e2b-events-openapi.yml
  format: yaml
  label: E2B Sandbox Events and Webhooks API
  slug: e2b-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-events-openapi.yml
- filename: e2b-api-openapi.yml
  format: yaml
  label: E2B Team and Identity API
  slug: e2b-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: e2b.dev
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: e2b.app
  spf: false
hosts:
- cert_expires: Aug 25 05:10:37 2026 GMT
  host: e2b.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 14:51:06 2026 GMT
  host: api.e2b.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: E2B Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for E2B, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: E2B
provider_slug: e2b-dev
slug: e2b-dev-domain-security
source_filename: e2b-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: e2b.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 05:10:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.e2b.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 14:51:06 2026 GMT\n  hsts: null\ndomains:\n- domain: e2b.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: e2b.app\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/security/e2b-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Agents
- Code Execution
- Code Interpreter
- Sandboxes
- Firecracker
- microVMs
- Computer Use
- Desktop Sandbox
- Templates
- MCP
- Open Source
---
