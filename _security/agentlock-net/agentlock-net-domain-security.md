---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agentlock.net
  spf: true
hosts:
- cert_expires: Jan 13 14:38:24 2027 GMT
  host: agentlock.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentlock Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentLock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AgentLock
provider_slug: agentlock-net
slug: agentlock-net-domain-security
source_filename: agentlock-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentlock.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 14:38:24 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agentlock.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/agentlock-net/security/agentlock-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Security
- Zero Trust
- API Gateway
- Agent Management
- Audit Trail
- Mobile approvals
---
