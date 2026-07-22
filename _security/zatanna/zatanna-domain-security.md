---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zatanna.ai
  spf: true
hosts:
- cert_expires: Sep 17 22:54:43 2026 GMT
  host: www.zatanna.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 02:12:34 2026 GMT
  host: api.zatanna.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zatanna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zatanna, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zatanna
provider_slug: zatanna
slug: zatanna-domain-security
source_filename: zatanna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zatanna.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 22:54:43 2026 GMT\n  hsts: false\n- host: api.zatanna.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 02:12:34 2026 GMT\n  hsts: null\ndomains:\n- domain: zatanna.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zatanna/refs/heads/main/security/zatanna-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- API
- MCP
- AI Agents
- Integration
- Reverse Engineering
- Automation
- OAuth
- Y Combinator
---
