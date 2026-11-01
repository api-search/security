---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pangea.io
  spf: true
hosts:
- cert_expires: Nov 27 03:18:14 2026 GMT
  host: www.pangea.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pangea Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pangea, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pangea
provider_slug: pangea-io
slug: pangea-io-domain-security
source_filename: pangea-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pangea.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 03:18:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pangea.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/pangea-io/security/pangea-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- Risk Management
- FX Hedging
- AI
---
