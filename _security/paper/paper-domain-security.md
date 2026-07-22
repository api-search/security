---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paper.design
  spf: true
hosts:
- cert_expires: Sep 26 11:26:45 2026 GMT
  host: paper.design
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paper, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Paper
provider_slug: paper
slug: paper-domain-security
source_filename: paper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paper.design\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 11:26:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: paper.design\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paper/refs/heads/main/security/paper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Design
- Design Tools
- MCP
- Agents
- HTML
- CSS
- Developer Tools
- Design to Code
---
