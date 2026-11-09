---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentbase.tools
  spf: false
hosts:
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: agentbase.tools
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentbase Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentBase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AgentBase
provider_slug: agentbase-tools
slug: agentbase-tools-domain-security
source_filename: agentbase-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentbase.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: agentbase.tools\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agentbase-tools/security/agentbase-tools-domain-security.yml
summary_line: TLSv1.3
tags:
- Knowledge Base
- Artificial Intelligence
- Collaboration
- Open Source
- Community
- Company
---
