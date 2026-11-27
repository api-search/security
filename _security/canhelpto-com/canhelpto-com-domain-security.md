---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: canhelpto.com
  spf: true
hosts:
- cert_expires: Jan  6 16:04:47 2027 GMT
  host: canhelpto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: canhelpto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for canhelpto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: canhelpto
provider_slug: canhelpto-com
slug: canhelpto-com-domain-security
source_filename: canhelpto-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: canhelpto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 16:04:47 2027 GMT\n  hsts: false\ndomains:\n- domain: canhelpto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/canhelpto-com/security/canhelpto-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Customer Service
- AI Integration
- MCP Server
- Help Desk
- Automation
---
