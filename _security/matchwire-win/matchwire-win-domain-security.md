---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: matchwire.win
  spf: true
hosts:
- cert_expires: Dec 28 11:39:00 2026 GMT
  host: matchwire.win
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Matchwire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matchwire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Matchwire
provider_slug: matchwire-win
slug: matchwire-win-domain-security
source_filename: matchwire-win-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: matchwire.win\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 11:39:00 2026 GMT\n  hsts: false\ndomains:\n- domain: matchwire.win\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/matchwire-win/security/matchwire-win-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Prediction Markets
- Market Data
- Sports Betting
- Real-Time Streaming
- Alias Mapping
- Commercial License
---
