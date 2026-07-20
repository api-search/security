---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: craft.do
  spf: true
hosts:
- cert_expires: Sep  6 23:58:00 2026 GMT
  host: www.craft.do
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Craft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for craft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: craft
provider_slug: craft
slug: craft-domain-security
source_filename: craft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.craft.do\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:58:00 2026 GMT\n  hsts: false\ndomains:\n- domain: craft.do\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/craft/refs/heads/main/security/craft-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Productivity
- Notes
- Documents
- Note Taking
- Tasks
- Collaboration
- Writing
- AI
- MCP
- Extensions
---
