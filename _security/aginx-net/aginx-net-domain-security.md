---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aginx.net
  spf: true
hosts:
- cert_expires: Jan 21 22:06:27 2027 GMT
  host: aginx.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aginx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aginx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aginx
provider_slug: aginx-net
slug: aginx-net-domain-security
source_filename: aginx-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aginx.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 22:06:27 2027 GMT\n  hsts: false\ndomains:\n- domain: aginx.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aginx-net/security/aginx-net-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Open Source
- Infrastructure
- Agent Network
- API Platform
---
