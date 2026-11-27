---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentworld.io
  spf: false
hosts:
- cert_expires: Feb  8 06:28:21 2027 GMT
  host: agentworld.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 08:46:38 2027 GMT
  host: play.agentworld.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: AgentWorld Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentWorld, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AgentWorld
provider_slug: agentworld-io
slug: agentworld-io-domain-security
source_filename: agentworld-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentworld.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 06:28:21 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: play.agentworld.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 08:46:38 2027 GMT\n  hsts: false\ndomains:\n- domain: agentworld.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agentworld-io/security/agentworld-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI Agents
- Multi-Agent Systems
- Benchmarks
- LLM Evaluation
- Games
- Open Source
---
