---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: foldlaboratories.com
  spf: true
hosts:
- cert_expires: Feb  2 03:24:41 2027 GMT
  host: foldlaboratories.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fold Laboratories Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fold Laboratories, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fold Laboratories
provider_slug: foldlaboratories-com
slug: foldlaboratories-com-domain-security
source_filename: foldlaboratories-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foldlaboratories.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 03:24:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: foldlaboratories.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/foldlaboratories-com/security/foldlaboratories-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Art
- Marketplace
- Artificial Intelligence
- Agents
- Original-Art
- Company
---
