---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kondux.io
  spf: true
hosts:
- cert_expires: Jan 30 18:51:12 2027 GMT
  host: kondux.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kondux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kondux, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kondux
provider_slug: kondux-io
slug: kondux-io-domain-security
source_filename: kondux-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kondux.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 18:51:12 2027 GMT\n  hsts: null\ndomains:\n- domain: kondux.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kondux-io/security/kondux-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Finance
- Security
- Agentic Commerce
- Blockchain
- NFT
---
