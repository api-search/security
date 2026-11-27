---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cambrian.org
  spf: true
hosts:
- cert_expires: Jan 24 22:10:33 2027 GMT
  host: cambrian.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cambrian Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cambrian Network, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cambrian Network
provider_slug: cambrian-org
slug: cambrian-org-domain-security
source_filename: cambrian-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cambrian.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 22:10:33 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cambrian.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cambrian-org/security/cambrian-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Digital Assets
- On-Chain Data
- Market Intelligence
- Cryptocurrency
---
