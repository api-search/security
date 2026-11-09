---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arthr.com.au
  spf: true
hosts:
- cert_expires: Dec  1 12:05:50 2026 GMT
  host: arthr.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arthr Com Au Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arthr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arthr
provider_slug: arthr-com-au
slug: arthr-com-au-domain-security
source_filename: arthr-com-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arthr.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 12:05:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: arthr.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/arthr-com-au/security/arthr-com-au-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mortgage
- Brokerage
- Artificial Intelligence
- Australia
- Fintech
---
