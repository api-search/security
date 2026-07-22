---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: betalist.com
  spf: true
hosts:
- cert_expires: Oct  9 16:39:05 2026 GMT
  host: betalist.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Betalist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BetaList, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BetaList
provider_slug: betalist
slug: betalist-domain-security
source_filename: betalist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: betalist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 16:39:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: betalist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betalist/refs/heads/main/security/betalist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Startups
- Beta Testing
- Product Discovery
- Early Adopters
- Newsletters
---
