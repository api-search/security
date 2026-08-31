---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentio.com
  spf: true
hosts:
- cert_expires: Nov  9 05:22:17 2026 GMT
  host: www.agentio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 12:03:18 2026 GMT
  host: mcp.agentio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agentio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agentio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agentio
provider_slug: agentio
slug: agentio-domain-security
source_filename: agentio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agentio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 05:22:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.agentio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 12:03:18 2026 GMT\n  hsts: null\ndomains:\n- domain: agentio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentio/refs/heads/main/security/agentio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Adtech
- Advertising
- Creator Economy
- Influencer Marketing
- Marketing
- Artificial Intelligence
- YouTube
- MCP
- Agents
- Analytics
---
