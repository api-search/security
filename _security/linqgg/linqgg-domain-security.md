---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: linq.gg
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: galactica.games
  spf: true
hosts:
- cert_expires: Oct  4 11:49:50 2026 GMT
  host: docs.linq.gg
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 15:56:53 2026 GMT
  host: services.galactica.games
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linqgg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linq.gg, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Linq.gg
provider_slug: linqgg
slug: linqgg-domain-security
source_filename: linqgg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.linq.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 11:49:50 2026 GMT\n  hsts: false\n- host: services.galactica.games\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 15:56:53 2026 GMT\n  hsts: null\ndomains:\n- domain: linq.gg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: galactica.games\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linqgg/refs/heads/main/security/linqgg-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gaming
- Payments
- Wallet
- Loyalty
- Fintech
- Real Money Gaming
- gRPC
- Geolocation
- Authentication
---
