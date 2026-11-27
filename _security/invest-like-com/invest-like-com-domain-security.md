---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: invest-like.com
  spf: true
hosts:
- cert_expires: Jan 12 10:55:45 2027 GMT
  host: invest-like.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Invest Like Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Invest Like, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Invest Like
provider_slug: invest-like-com
slug: invest-like-com-domain-security
source_filename: invest-like-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: invest-like.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 10:55:45 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: invest-like.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/invest-like-com/security/invest-like-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Artificial Intelligence
- Stock Analysis
- Portfolio
- Investment
---
