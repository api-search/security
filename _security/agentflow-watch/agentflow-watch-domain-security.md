---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentflow.watch
  spf: false
hosts:
- cert_expires: Jan 12 08:01:48 2027 GMT
  host: agentflow.watch
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentflow Watch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentFlow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AgentFlow
provider_slug: agentflow-watch
slug: agentflow-watch-domain-security
source_filename: agentflow-watch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentflow.watch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 08:01:48 2027 GMT\n  hsts: false\ndomains:\n- domain: agentflow.watch\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agentflow-watch/security/agentflow-watch-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Finance
- Blockchain
- Base
- USDC
- Monitoring
---
