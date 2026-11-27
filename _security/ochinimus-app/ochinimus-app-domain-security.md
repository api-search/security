---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ochinimus.app
  spf: true
hosts:
- cert_expires: Jan  9 09:06:49 2027 GMT
  host: ochinimus.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ochinimus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ochinimus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ochinimus
provider_slug: ochinimus-app
slug: ochinimus-app-domain-security
source_filename: ochinimus-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ochinimus.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 09:06:49 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ochinimus.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ochinimus-app/security/ochinimus-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Market Data
- Blockchain
- On-Chain-Payment
---
