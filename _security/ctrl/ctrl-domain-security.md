---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getctrl.co
  spf: false
hosts:
- cert_expires: Sep  1 11:33:04 2026 GMT
  host: www.getctrl.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ctrl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ctrl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Ctrl
provider_slug: ctrl
slug: ctrl-domain-security
source_filename: ctrl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getctrl.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 11:33:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getctrl.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ctrl/refs/heads/main/security/ctrl-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Sales
- Revenue Operations
- CRM
- Productivity
- Workspace
- Automation
- Artificial Intelligence
- SaaS
---
