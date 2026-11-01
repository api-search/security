---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stockmark.co.jp
  spf: true
hosts:
- cert_expires: Nov 23 02:18:09 2026 GMT
  host: stockmark.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stockmark Co Jp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stockmark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Stockmark
provider_slug: stockmark-co-jp
slug: stockmark-co-jp-domain-security
source_filename: stockmark-co-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stockmark.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 02:18:09 2026 GMT\n  hsts: false\ndomains:\n- domain: stockmark.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/stockmark-co-jp/security/stockmark-co-jp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Software-as-a-Service
- Platform-as-a-Service
- Knowledge Management
- Japan
---
