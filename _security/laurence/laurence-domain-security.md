---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: laurence.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: modal.run
  spf: true
hosts:
- cert_expires: Oct  1 20:40:07 2026 GMT
  host: www.laurence.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 12:20:35 2026 GMT
  host: laurence-ai-68564--ask-laurence-agent-mcp-server.modal.run
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Laurence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laurence, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Laurence
provider_slug: laurence
slug: laurence-domain-security
source_filename: laurence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.laurence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:40:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: laurence-ai-68564--ask-laurence-agent-mcp-server.modal.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 12:20:35 2026 GMT\n  hsts: null\ndomains:\n- domain: laurence.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: modal.run\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laurence/refs/heads/main/security/laurence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Amazon
- E-Commerce
- Marketing
- Machine Learning
- Retail Media
- MCP
---
