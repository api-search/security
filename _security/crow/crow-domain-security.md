---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: usecrow.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: usecrow.org
  spf: false
hosts:
- cert_expires: Oct  7 21:25:02 2026 GMT
  host: www.usecrow.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 10:30:14 2026 GMT
  host: docs.usecrow.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 22:07:27 2026 GMT
  host: api.usecrow.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crow, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Crow
provider_slug: crow
slug: crow-domain-security
source_filename: crow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usecrow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:25:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.usecrow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 10:30:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.usecrow.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 22:07:27 2026 GMT\n  hsts: null\ndomains:\n- domain: usecrow.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: usecrow.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crow/refs/heads/main/security/crow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- MCP
- Model Context Protocol
- OpenAPI
- Developer Tools
- SDK
- Embeddable Widget
- Commercial Real Estate
---
