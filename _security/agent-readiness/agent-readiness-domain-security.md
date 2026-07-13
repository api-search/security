---
api_specs:
- filename: openapi
  format: yaml
  label: Stripe API (reference provider)
  slug: stripe-api
  spec_type: OpenAPI
  url: https://github.com/stripe/openapi
- filename: rest-api-description
  format: yaml
  label: GitHub REST + GraphQL API (reference provider)
  slug: github-rest-api
  spec_type: OpenAPI
  url: https://github.com/github/rest-api-description
- filename: twilio-oai
  format: yaml
  label: Twilio API (reference provider)
  slug: twilio-api
  spec_type: OpenAPI
  url: https://github.com/twilio/twilio-oai
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: modelcontextprotocol.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openapis.org
  spf: true
hosts:
- cert_expires: Sep  1 00:36:56 2026 GMT
  host: modelcontextprotocol.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 18:54:28 2026 GMT
  host: www.openapis.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 05:12:18 2026 GMT
  host: spec.openapis.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agent Readiness Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Readiness, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agent Readiness
provider_slug: agent-readiness
slug: agent-readiness-domain-security
source_filename: agent-readiness-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modelcontextprotocol.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 00:36:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.openapis.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:54:28 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: spec.openapis.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 05:12:18 2026 GMT\n  hsts: false\ndomains:\n- domain: modelcontextprotocol.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: openapis.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agent-readiness/refs/heads/main/security/agent-readiness-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agent Readiness
- AI Agents
- API Discovery
- API Governance
- Machine-Readable APIs
- MCP
- OpenAPI
- AsyncAPI
---
