---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: coinmetro.com
  spf: true
hosts:
- cert_expires: Nov 12 22:58:28 2026 GMT
  host: www.coinmetro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coinmetro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coinmetro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Coinmetro
provider_slug: coinmetro
slug: coinmetro-domain-security
source_filename: coinmetro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coinmetro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 22:58:28 2026 GMT\n  hsts: false\ndomains:\n- domain: coinmetro.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinmetro/refs/heads/main/security/coinmetro-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Spot Trading
- Margin Trading
- Staking
- Auto Invest
---
