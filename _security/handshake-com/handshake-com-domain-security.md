---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: handshake.com
  spf: true
hosts:
- cert_expires: Jan  7 15:40:55 2027 GMT
  host: www.handshake.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Handshake Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for handshake, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: handshake
provider_slug: handshake-com
slug: handshake-com-domain-security
source_filename: handshake-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.handshake.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 15:40:55 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: handshake.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/handshake-com/security/handshake-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Marketplace
- Wholesale
- Suppliers
- E-commerce
---
