---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: marketaxess.com
  spf: true
hosts:
- cert_expires: Nov 27 03:53:11 2026 GMT
  host: www.marketaxess.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Marketaxess Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MarketAxess, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MarketAxess
provider_slug: marketaxess
slug: marketaxess-domain-security
source_filename: marketaxess-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.marketaxess.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 03:53:11 2026 GMT\n  hsts: false\ndomains:\n- domain: marketaxess.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketaxess/refs/heads/main/security/marketaxess-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- Trading
- Bonds
---
