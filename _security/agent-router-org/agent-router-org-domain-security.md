---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agent-router.org
  spf: true
hosts:
- cert_expires: Jan  6 01:19:40 2027 GMT
  host: agent-router.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agent Router Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentRouter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AgentRouter
provider_slug: agent-router-org
slug: agent-router-org-domain-security
source_filename: agent-router-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agent-router.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 01:19:40 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agent-router.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agent-router-org/security/agent-router-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- MCP
- Integration
- Platform
---
