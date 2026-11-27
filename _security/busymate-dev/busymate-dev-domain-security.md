---
api_specs:
- filename: busymate-dev-core-openapi-generated.yml
  format: yaml
  label: Busymate DevTools core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/busymate-dev/openapi/_ae-authored/busymate-dev-core-openapi-generated.yml
- filename: busymate-dev-federation-openapi-generated.yml
  format: yaml
  label: Busymate DevTools federation API
  slug: federation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/busymate-dev/openapi/_ae-authored/busymate-dev-federation-openapi-generated.yml
- filename: busymate-dev-mcp-openapi-generated.yml
  format: yaml
  label: Busymate DevTools mcp API
  slug: mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/busymate-dev/openapi/_ae-authored/busymate-dev-mcp-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: busymate.dev
  spf: true
hosts:
- cert_expires: Jan 14 09:33:37 2027 GMT
  host: busymate.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Busymate DevTools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Busymate DevTools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Busymate DevTools
provider_slug: busymate-dev
slug: busymate-dev-domain-security
source_filename: busymate-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: busymate.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 09:33:37 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: busymate.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/busymate-dev/security/busymate-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- Network Monitoring
- HTTPS Debugging
- AI Assistance
- Mobile Development
---
