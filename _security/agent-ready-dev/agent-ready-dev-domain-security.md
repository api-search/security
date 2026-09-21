---
api_specs:
- filename: agent-ready-dev-openapi.yml
  format: yaml
  label: Agent Ready API
  slug: agent-ready-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agent-ready-dev/refs/heads/main/openapi/agent-ready-dev-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: agent-ready.dev
  spf: true
hosts:
- cert_expires: Nov 17 05:04:30 2026 GMT
  host: agent-ready.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agent Ready Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Ready, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Agent Ready
provider_slug: agent-ready-dev
slug: agent-ready-dev-domain-security
source_filename: agent-ready-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agent-ready.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 05:04:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agent-ready.dev\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agent-ready-dev/refs/heads/main/security/agent-ready-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agents
- Agent Readiness
- Website Scanning
- Developer Tools
- MCP
- A2A
- llms-txt
- x402
- NLWeb
- Accessibility
- agent-native
- Australia
---
