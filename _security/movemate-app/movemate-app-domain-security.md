---
api_specs:
- filename: movemate-app-health-api-openapi.yml
  format: yaml
  label: MoveMate Health API
  slug: movemate-app-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movemate-app/openapi/movemate-app-health-api-openapi.yml
- filename: movemate-app-mcp-api-openapi.yml
  format: yaml
  label: MoveMate MCP API
  slug: movemate-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movemate-app/openapi/movemate-app-mcp-api-openapi.yml
- filename: movemate-app-oauth-api-openapi.yml
  format: yaml
  label: MoveMate OAuth API
  slug: movemate-app-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movemate-app/openapi/movemate-app-oauth-api-openapi.yml
description: ''
domains:
- caa:
  - shboj62d.up.railway.app.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: movemate.app
  spf: true
hosts:
- cert_expires: Jan  5 05:48:59 2027 GMT
  host: movemate.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MoveMate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MoveMate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: MoveMate
provider_slug: movemate-app
slug: movemate-app-domain-security
source_filename: movemate-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: movemate.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 05:48:59 2027 GMT\n  hsts: false\ndomains:\n- domain: movemate.app\n  dnssec: true\n  caa:\n  - shboj62d.up.railway.app.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/movemate-app/security/movemate-app-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Fitness
- Artificial Intelligence
- Workouts
- Health
- Mobile
---
