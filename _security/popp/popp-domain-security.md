---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: joinpopp.com
  spf: true
hosts:
- cert_expires: Oct 15 10:16:54 2026 GMT
  host: joinpopp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Popp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Popp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Popp
provider_slug: popp
slug: popp-domain-security
source_filename: popp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joinpopp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 10:16:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: joinpopp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/security/popp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Recruitment
- Staffing
- Hiring
- Conversational AI
- Automation
- Scheduling
- Workflows
- Webhooks
- MCP
- Agents
---
