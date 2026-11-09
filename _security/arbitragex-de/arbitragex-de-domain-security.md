---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arbitragex.de
  spf: true
hosts:
- cert_expires: Dec 28 14:25:07 2026 GMT
  host: arbitragex.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arbitragex De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arbitragex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arbitragex
provider_slug: arbitragex-de
slug: arbitragex-de-domain-security
source_filename: arbitragex-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arbitragex.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 14:25:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arbitragex.de\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/arbitragex-de/security/arbitragex-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon
- Arbitrage
- FBA
- Profit
- Automation
- SP-API
---
