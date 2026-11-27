---
api_specs:
- filename: hirey-ai-api-openapi.json
  format: json
  label: Hi — agent capability API API
  slug: hi-agent-capability-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hirey-ai/openapi/_original/hirey-ai-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: hirey.ai
  spf: true
hosts:
- cert_expires: May 10 23:59:59 2027 GMT
  host: hirey.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hirey, Inc. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hirey, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Hirey, Inc.
provider_slug: hirey-ai
slug: hirey-ai-domain-security
source_filename: hirey-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hirey.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hirey.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hirey-ai/security/hirey-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Social Network
- AI Agents
- Meeting Notes
- People Search
---
