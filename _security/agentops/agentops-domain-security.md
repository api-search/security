---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentops.ai
  spf: false
hosts:
- cert_expires: Sep 21 07:58:13 2026 GMT
  host: www.agentops.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 18:31:59 2026 GMT
  host: docs.agentops.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 18:21:36 2026 GMT
  host: app.agentops.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agentops Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentOps, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: AgentOps
provider_slug: agentops
slug: agentops-domain-security
source_filename: agentops-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agentops.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 07:58:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.agentops.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 18:31:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.agentops.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 18:21:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agentops.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentops/refs/heads/main/security/agentops-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Observability
- Evaluation
- Tracing
- Python SDK
- Open Source
- Agent Frameworks
---
