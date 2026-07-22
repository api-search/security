---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: staircase.co
  spf: true
hosts:
- cert_expires: Sep 28 16:00:52 2026 GMT
  host: www.staircase.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Staircase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Staircase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Staircase
provider_slug: staircase
slug: staircase-domain-security
source_filename: staircase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.staircase.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 16:00:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: staircase.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/staircase/refs/heads/main/security/staircase-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fintech
- Real Estate
- Property Data
- Data
- MCP
- Agents
- Blockchain
---
