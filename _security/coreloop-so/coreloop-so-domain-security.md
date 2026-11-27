---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coreloop.so
  spf: false
hosts:
- cert_expires: Dec 25 03:30:53 2026 GMT
  host: coreloop.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CoreLoop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoreLoop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: CoreLoop
provider_slug: coreloop-so
slug: coreloop-so-domain-security
source_filename: coreloop-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coreloop.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 03:30:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coreloop.so\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/coreloop-so/security/coreloop-so-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- MCP
- A2A
- Llms.txt
- Business Directory
- Agent Discoverability
---
