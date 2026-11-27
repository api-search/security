---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: copywriting.sh
  spf: false
hosts:
- cert_expires: Jan 22 23:50:40 2027 GMT
  host: copywriting.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Copywriting MCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Copywriting MCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Copywriting MCP
provider_slug: copywriting-sh
slug: copywriting-sh-domain-security
source_filename: copywriting-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: copywriting.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:50:40 2027 GMT\n  hsts: false\ndomains:\n- domain: copywriting.sh\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/copywriting-sh/security/copywriting-sh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Copywriting
- MCP
- AI Agents
- Knowledge Base
- Marketing
- Content Writing
---
