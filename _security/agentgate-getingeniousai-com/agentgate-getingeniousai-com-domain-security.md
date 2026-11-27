---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getingeniousai.com
  spf: true
hosts:
- cert_expires: Jan 19 21:56:34 2027 GMT
  host: agentgate.getingeniousai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AgentGate (Ingenious AI) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentGate (Ingenious AI), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AgentGate (Ingenious AI)
provider_slug: agentgate-getingeniousai-com
slug: agentgate-getingeniousai-com-domain-security
source_filename: agentgate-getingeniousai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentgate.getingeniousai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 21:56:34 2027 GMT\n  hsts: false\ndomains:\n- domain: getingeniousai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agentgate-getingeniousai-com/security/agentgate-getingeniousai-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Policy
- Governance
- Software-as-a-Service
---
