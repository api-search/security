---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: axel.trade
  spf: true
hosts:
- cert_expires: Jan 10 11:47:19 2027 GMT
  host: axel.trade
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Axel Trade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for axel-trade, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: axel-trade
provider_slug: axel-trade
slug: axel-trade-domain-security
source_filename: axel-trade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axel.trade\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 11:47:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: axel.trade\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/axel-trade/security/axel-trade-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Finance
- Tax
- Accounting
- Software
- UK
---
