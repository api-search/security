---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bstock.com
  spf: true
hosts:
- cert_expires: Dec 20 10:56:48 2026 GMT
  host: bstock.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: B Stock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for B-Stock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: B-Stock
provider_slug: b-stock
slug: b-stock-domain-security
source_filename: b-stock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bstock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 10:56:48 2026 GMT\n  hsts: null\ndomains:\n- domain: bstock.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/b-stock/security/b-stock-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- liquidation
- wholesale
- inventory resale
- auction
- buy now
- net terms
---
