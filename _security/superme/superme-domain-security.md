---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: superme.ai
  spf: true
hosts:
- cert_expires: Oct 18 17:41:42 2026 GMT
  host: superme.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SuperMe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SuperMe
provider_slug: superme
slug: superme-domain-security
source_filename: superme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: superme.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 17:41:42 2026 GMT\n  hsts: false\ndomains:\n- domain: superme.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superme/refs/heads/main/security/superme-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Professional Network
- Expert Knowledge
- Model Context Protocol
- MCP
---
