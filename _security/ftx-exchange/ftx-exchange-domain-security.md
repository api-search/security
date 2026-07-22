---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ftx.us
  spf: true
hosts:
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: ftx.us
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ftx Exchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FTX Exchange, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FTX Exchange
provider_slug: ftx-exchange
slug: ftx-exchange-domain-security
source_filename: ftx-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ftx.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ftx.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ftx-exchange/refs/heads/main/security/ftx-exchange-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Web3
---
