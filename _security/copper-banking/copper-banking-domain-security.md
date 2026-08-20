---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getcopper.com
  spf: true
hosts:
- cert_expires: Sep 30 14:01:49 2026 GMT
  host: www.getcopper.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 01:40:51 2026 GMT
  host: mcp.getcopper.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Copper Banking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Copper Banking, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Copper Banking
provider_slug: copper-banking
slug: copper-banking-domain-security
source_filename: copper-banking-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getcopper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:01:49 2026 GMT\n  hsts: null\n- host: mcp.getcopper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 01:40:51 2026 GMT\n  hsts: null\ndomains:\n- domain: getcopper.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/copper-banking/refs/heads/main/security/copper-banking-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial-Services
- Fintech
- Consumer Finance
- Financial Literacy
- Rewards
- Neobank
- Mobile Banking
- Teen Banking
- MCP
---
