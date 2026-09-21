---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: meshgateway.app
  spf: false
hosts:
- cert_expires: Dec 15 01:30:25 2026 GMT
  host: meshgateway.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Meshgateway App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for William, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: William
provider_slug: meshgateway-app
slug: meshgateway-app-domain-security
source_filename: meshgateway-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meshgateway.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 01:30:25 2026 GMT\n  hsts: false\ndomains:\n- domain: meshgateway.app\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meshgateway-app/refs/heads/main/security/meshgateway-app-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Agents
- A2A
- Agent Card
- Discord
- Chat
- Multi-Agent
- Agent Mesh
---
