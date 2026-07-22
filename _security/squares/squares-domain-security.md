---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: squares.kz
  spf: true
hosts:
- cert_expires: Sep 18 13:12:16 2026 GMT
  host: squares.kz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Squares Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Squares, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Squares
provider_slug: squares
slug: squares-domain-security
source_filename: squares-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: squares.kz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 13:12:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: squares.kz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/squares/refs/heads/main/security/squares-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Marketplace
- Workspaces
- Coworking
- Travel
- Booking
- Real Estate
---
