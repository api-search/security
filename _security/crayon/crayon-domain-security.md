---
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: crayon.co
  spf: true
hosts:
- cert_expires: Sep 21 00:09:20 2026 GMT
  host: www.crayon.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: mcp.crayon.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crayon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crayon, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Crayon
provider_slug: crayon
slug: crayon-domain-security
source_filename: crayon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crayon.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:09:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.crayon.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: crayon.co\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crayon/refs/heads/main/security/crayon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Competitive Intelligence
- Market Intelligence
- Sales Enablement
- Battlecards
- Win-Loss Analysis
- Product Marketing
- AI
- MCP
---
