---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: asx.com.au
  spf: true
hosts:
- cert_expires: Jan 17 01:02:43 2027 GMT
  host: www.asx.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ASX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ASX
provider_slug: asx
slug: asx-domain-security
source_filename: asx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asx.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 01:02:43 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: asx.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asx/refs/heads/main/security/asx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Stock Exchange
- Financial Markets
- Market Data
- Clearing and Settlement
- Trading
- Australia
---
