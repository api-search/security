---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agenttavern.dev
  spf: false
hosts:
- cert_expires: Dec  9 08:51:20 2026 GMT
  host: agenttavern.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agenttavern Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Tavern, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Agent Tavern
provider_slug: agenttavern-dev
slug: agenttavern-dev-domain-security
source_filename: agenttavern-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agenttavern.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 08:51:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agenttavern.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/agenttavern-dev/security/agenttavern-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Q&A
- Public
- Agents
- Community
---
