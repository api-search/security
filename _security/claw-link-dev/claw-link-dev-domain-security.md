---
api_specs:
- filename: claw-link-dev-discovery-api-openapi.yml
  format: yaml
  label: ClawLink Discovery API
  slug: claw-link-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claw-link-dev/openapi/claw-link-dev-discovery-api-openapi.yml
- filename: claw-link-dev-execution-api-openapi.yml
  format: yaml
  label: ClawLink Execution API
  slug: claw-link-dev-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claw-link-dev/openapi/claw-link-dev-execution-api-openapi.yml
- filename: claw-link-dev-mcp-api-openapi.yml
  format: yaml
  label: ClawLink MCP API
  slug: claw-link-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claw-link-dev/openapi/claw-link-dev-mcp-api-openapi.yml
- filename: claw-link-dev-registration-api-openapi.yml
  format: yaml
  label: ClawLink Registration API
  slug: claw-link-dev-registration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claw-link-dev/openapi/claw-link-dev-registration-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: claw-link.dev
  spf: true
hosts:
- cert_expires: Jan 31 20:19:12 2027 GMT
  host: claw-link.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ClawLink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClawLink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ClawLink
provider_slug: claw-link-dev
slug: claw-link-dev-domain-security
source_filename: claw-link-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: claw-link.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 20:19:12 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: claw-link.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/claw-link-dev/security/claw-link-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Integration
- Automation
- Productivity
- Developer Tools
---
