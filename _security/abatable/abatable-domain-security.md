---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: abatable.com
  spf: true
hosts:
- cert_expires: Nov  7 14:32:20 2026 GMT
  host: abatable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 17:01:21 2026 GMT
  host: mcp.abatable.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Abatable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abatable, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Abatable
provider_slug: abatable
slug: abatable-domain-security
source_filename: abatable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abatable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 14:32:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.abatable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 17:01:21 2026 GMT\n  hsts: null\ndomains:\n- domain: abatable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abatable/refs/heads/main/security/abatable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Carbon Markets
- Carbon Credits
- Carbon Offsets
- Environmental Assets
- Voluntary Carbon Market
- CORSIA
- Climate
- Sustainability
- Net Zero
- Procurement
- Market Intelligence
- Due Diligence
- ESG
- MCP
---
