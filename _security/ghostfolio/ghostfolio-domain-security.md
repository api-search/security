---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ghostfol.io
  spf: true
hosts:
- cert_expires: Dec 24 17:07:53 2026 GMT
  host: ghostfol.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ghostfolio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ghostfolio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ghostfolio
provider_slug: ghostfolio
slug: ghostfolio-domain-security
source_filename: ghostfolio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ghostfol.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 17:07:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ghostfol.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ghostfolio/security/ghostfolio-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Finance
- Wealth Management
- Open Source
- SaaS
- Portfolio
---
