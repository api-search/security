---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: masaro.ai
  spf: true
hosts:
- cert_expires: Jan 14 07:05:21 2027 GMT
  host: masaro.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Masaro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Masaro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Masaro
provider_slug: masaro-ai
slug: masaro-ai-domain-security
source_filename: masaro-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: masaro.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 07:05:21 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: masaro.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/masaro-ai/security/masaro-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Task Management
- AI Agents
- software teams
- Project Planning
- MCP integration
---
