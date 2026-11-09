---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: carrierscore.io
  spf: true
hosts:
- cert_expires: Jan 12 21:47:21 2027 GMT
  host: carrierscore.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carrierscore Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CarrierScore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CarrierScore
provider_slug: carrierscore-io
slug: carrierscore-io-domain-security
source_filename: carrierscore-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carrierscore.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 21:47:21 2027 GMT\n  hsts: false\ndomains:\n- domain: carrierscore.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/carrierscore-io/security/carrierscore-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Freight
- Logistics
- Risk Management
- Data
---
