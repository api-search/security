---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hockeytech.com
  spf: true
hosts:
- cert_expires: Jan 20 04:22:07 2027 GMT
  host: hockeytech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hockeytech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HockeyTech league feed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HockeyTech league feed
provider_slug: hockeytech
slug: hockeytech-domain-security
source_filename: hockeytech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hockeytech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 04:22:07 2027 GMT\n  hsts: false\ndomains:\n- domain: hockeytech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hockeytech/security/hockeytech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Sports
- Data
- Analytics
- Streaming
- API
---
