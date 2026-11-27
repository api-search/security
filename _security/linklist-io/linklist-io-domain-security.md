---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: linklist.io
  spf: true
hosts:
- cert_expires: Feb  4 15:32:25 2027 GMT
  host: linklist.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TrueStandard Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrueStandard Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TrueStandard Labs
provider_slug: linklist-io
slug: linklist-io-domain-security
source_filename: linklist-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linklist.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 15:32:25 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: linklist.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/linklist-io/security/linklist-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Data
- Platform
- MCP
- Collection
---
