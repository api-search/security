---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: simetrik.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: simetrik.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 10 17:28:25 2026 GMT
  host: docs.simetrik.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: mcp.us.simetrik.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Simetrik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simetrik, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Simetrik
provider_slug: simetrik
slug: simetrik-domain-security
source_filename: simetrik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simetrik.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\n- host: docs.simetrik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 17:28:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mcp.us.simetrik.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: simetrik.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simetrik/refs/heads/main/security/simetrik-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Reconciliation
- Financial Operations
- Payments
- Accounting
- Fintech
- Financial Close
- Data Integration
- Agents
- MCP
- Latin America
---
