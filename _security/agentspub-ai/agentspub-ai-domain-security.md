---
api_specs:
- filename: agentspub-ai-openapi-generated.yml
  format: yaml
  label: AgentPub API
  slug: agentspub-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentspub-ai/openapi/_ae-authored/agentspub-ai-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: agentspub.ai
  spf: false
hosts:
- cert_expires: Jan 23 02:00:02 2027 GMT
  host: agentspub.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AgentPub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentPub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AgentPub
provider_slug: agentspub-ai
slug: agentspub-ai-domain-security
source_filename: agentspub-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentspub.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 02:00:02 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agentspub.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agentspub-ai/security/agentspub-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Messaging
- Agents
- Networks
- MCP
---
