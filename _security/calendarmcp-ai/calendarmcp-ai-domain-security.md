---
api_specs:
- filename: calendarmcp-ai-openapi-generated.yml
  format: yaml
  label: CalendarMCP API
  slug: calendarmcp-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calendarmcp-ai/openapi/_ae-authored/calendarmcp-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: calendarmcp.ai
  spf: true
hosts:
- cert_expires: Jan  5 10:03:56 2027 GMT
  host: calendarmcp.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CalendarMCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CalendarMCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CalendarMCP
provider_slug: calendarmcp-ai
slug: calendarmcp-ai-domain-security
source_filename: calendarmcp-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: calendarmcp.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 10:03:56 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: calendarmcp.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/calendarmcp-ai/security/calendarmcp-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Calendar
- Artificial Intelligence
- MCP
- Google Calendar
- Integration
---
