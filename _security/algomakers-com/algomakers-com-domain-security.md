---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: algomakers.com
  spf: true
hosts:
- cert_expires: Nov 29 00:43:09 2026 GMT
  host: algomakers.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Algomakers Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AlgoMaker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AlgoMaker
provider_slug: algomakers-com
slug: algomakers-com-domain-security
source_filename: algomakers-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: algomakers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 00:43:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: algomakers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/algomakers-com/security/algomakers-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Quantitative Trading
- AI Agents
- MCP
- Finance
- Institutional
---
