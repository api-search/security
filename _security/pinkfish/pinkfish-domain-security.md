---
api_specs:
- filename: pinkfish-triggers-openapi.yml
  format: yaml
  label: Pinkfish Triggers API
  slug: pinkfish-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinkfish/refs/heads/main/openapi/pinkfish-triggers-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pinkfish.ai
  spf: true
hosts:
- cert_expires: Oct  3 05:15:05 2026 GMT
  host: pinkfish.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 04:03:24 2026 GMT
  host: docs.pinkfish.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: triggers.app.pinkfish.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pinkfish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pinkfish, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pinkfish
provider_slug: pinkfish
slug: pinkfish-domain-security
source_filename: pinkfish-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pinkfish.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 05:15:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pinkfish.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 04:03:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: triggers.app.pinkfish.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: pinkfish.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinkfish/refs/heads/main/security/pinkfish-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agentic Workflows
- Automation
- Orchestration
- Model Context Protocol
- Integrations
- Enterprise
- No-Code
---
