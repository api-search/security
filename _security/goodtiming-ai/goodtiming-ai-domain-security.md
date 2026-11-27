---
api_specs:
- filename: goodtiming-ai-metrics-api-openapi.yml
  format: yaml
  label: Good Timing Metrics API
  slug: goodtiming-ai-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodtiming-ai/openapi/goodtiming-ai-metrics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: goodtiming.ai
  spf: true
hosts:
- cert_expires: Dec 19 04:39:17 2026 GMT
  host: goodtiming.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Good Timing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Good Timing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Good Timing
provider_slug: goodtiming-ai
slug: goodtiming-ai-domain-security
source_filename: goodtiming-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goodtiming.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 04:39:17 2026 GMT\n  hsts: false\ndomains:\n- domain: goodtiming.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/goodtiming-ai/security/goodtiming-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- MCP
- Product Analytics
- AI Agents
- Observability
- SDK
---
