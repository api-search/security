---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentgid.com
  spf: true
hosts:
- cert_expires: Jan  4 00:51:09 2027 GMT
  host: agentgid.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentgid Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentGid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AgentGid
provider_slug: agentgid-com
slug: agentgid-com-domain-security
source_filename: agentgid-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentgid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 00:51:09 2027 GMT\n  hsts: false\ndomains:\n- domain: agentgid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agentgid-com/security/agentgid-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Agents
- Data
- Marketplace
- Analytics
---
