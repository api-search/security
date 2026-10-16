---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: coinflip.tech
  spf: true
hosts:
- cert_expires: Jan  1 19:09:40 2027 GMT
  host: coinflip.tech
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 05:01:20 2026 GMT
  host: app.coinflip.tech
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Coinflipsolutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coinflipsolutions, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Coinflipsolutions
provider_slug: coinflipsolutions
slug: coinflipsolutions-domain-security
source_filename: coinflipsolutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coinflip.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 19:09:40 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: app.coinflip.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 05:01:20 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: coinflip.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinflipsolutions/refs/heads/main/security/coinflipsolutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
