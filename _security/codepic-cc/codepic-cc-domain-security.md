---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: codepic.cc
  spf: true
hosts:
- cert_expires: Dec 31 06:44:59 2026 GMT
  host: codepic.cc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CodePic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodePic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CodePic
provider_slug: codepic-cc
slug: codepic-cc-domain-security
source_filename: codepic-cc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codepic.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 06:44:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: codepic.cc\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/codepic-cc/security/codepic-cc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Whiteboard
- Diagramming
- Flowcharts
- MCP
- AI Agents
- Visual Collaboration
---
