---
api_specs:
- filename: e2b-dev-access-tokens-api-openapi.yml
  format: yaml
  label: E2B access-tokens API
  slug: e2b-dev-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-dev-access-tokens-api-openapi.yml
- filename: e2b-dev-admin-api-openapi.yml
  format: yaml
  label: E2B admin API
  slug: e2b-dev-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-dev-admin-api-openapi.yml
- filename: e2b-dev-api-keys-api-openapi.yml
  format: yaml
  label: E2B api-keys API
  slug: e2b-dev-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-dev-api-keys-api-openapi.yml
- filename: e2b-dev-auth-api-openapi.yml
  format: yaml
  label: E2B auth API
  slug: e2b-dev-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-dev-auth-api-openapi.yml
- filename: e2b-dev-events-api-openapi.yml
  format: yaml
  label: E2B events API
  slug: e2b-dev-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-dev-events-api-openapi.yml
- filename: e2b-dev-health-api-openapi.yml
  format: yaml
  label: E2B Health API
  slug: e2b-dev-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-dev-health-api-openapi.yml
- filename: e2b-dev-sandboxes-api-openapi.yml
  format: yaml
  label: E2B sandboxes API
  slug: e2b-dev-sandboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-dev-sandboxes-api-openapi.yml
- filename: e2b-dev-snapshots-api-openapi.yml
  format: yaml
  label: E2B snapshots API
  slug: e2b-dev-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-dev-snapshots-api-openapi.yml
- filename: e2b-dev-tags-api-openapi.yml
  format: yaml
  label: E2B tags API
  slug: e2b-dev-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-dev-tags-api-openapi.yml
- filename: e2b-dev-templates-api-openapi.yml
  format: yaml
  label: E2B templates API
  slug: e2b-dev-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-dev-templates-api-openapi.yml
- filename: e2b-dev-volumes-api-openapi.yml
  format: yaml
  label: E2B volumes API
  slug: e2b-dev-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-dev-volumes-api-openapi.yml
- filename: e2b-dev-webhooks-api-openapi.yml
  format: yaml
  label: E2B webhooks API
  slug: e2b-dev-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-dev-webhooks-api-openapi.yml
- filename: e2b-dev-e2b-sandbox-events-and-webhooks-api-api-openapi.yml
  format: yaml
  label: E2B E2B Sandbox Events And Webhooks API
  slug: e2b-dev-e2b-sandbox-events-and-webhooks-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2b-dev/refs/heads/main/openapi/e2b-dev-e2b-sandbox-events-and-webhooks-api-api-openapi.yml
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
- Artificial Intelligence
- Agents
- Code Execution
- Code Interpreter
- Sandboxes
- Firecracker
- MicroVMs
- Computer Use
- Desktop Sandbox
- Templates
- MCP
- Open-Source
---
