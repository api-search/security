---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentroam.ai
  spf: true
hosts:
- cert_expires: Jan 26 21:08:44 2027 GMT
  host: agentroam.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AgentRoam.ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentRoam.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AgentRoam.ai
provider_slug: agentroam-ai
slug: agentroam-ai-domain-security
source_filename: agentroam-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentroam.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 21:08:44 2027 GMT\n  hsts: false\ndomains:\n- domain: agentroam.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agentroam-ai/security/agentroam-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- eSIM
- Travel Data
- AI Agents
- Mobile Connectivity
---
