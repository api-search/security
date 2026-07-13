---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: oddsmagnet.com
  spf: false
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: data.oddsmagnet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oddsmagnet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oddsmagnet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Oddsmagnet
provider_slug: oddsmagnet
slug: oddsmagnet-domain-security
source_filename: oddsmagnet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.oddsmagnet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: oddsmagnet.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oddsmagnet/refs/heads/main/security/oddsmagnet-domain-security.yml
summary_line: TLSv1.3
tags:
- Sports And Fitness
- Public APIs
---
