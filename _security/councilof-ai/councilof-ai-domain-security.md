---
api_specs:
- filename: councilof-ai-public-api-openapi.yml
  format: yaml
  label: Council of AI Public API
  slug: council-of-ai-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/councilof-ai/refs/heads/main/openapi/councilof-ai-public-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: councilof.ai
  spf: false
hosts:
- cert_expires: Oct 30 11:05:57 2026 GMT
  host: councilof.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Councilof Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Council of AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Council of AI
provider_slug: councilof-ai
slug: councilof-ai-domain-security
source_filename: councilof-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: councilof.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 11:05:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: councilof.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/councilof-ai/refs/heads/main/security/councilof-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI Governance
- AI Measurement
- AI Safety
- EU AI Act
- Compliance
- Provenance
- Agents
- A2A
- MCP
- x402
- Agentic Commerce
- Agent-Native
- United Kingdom
---
