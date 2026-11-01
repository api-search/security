---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apdf.io
  spf: true
hosts:
- cert_expires: Dec 13 11:40:58 2026 GMT
  host: apdf.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apdf Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for apdf-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: apdf-io
provider_slug: apdf-io
slug: apdf-io-domain-security
source_filename: apdf-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apdf.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 11:40:58 2026 GMT\n  hsts: false\ndomains:\n- domain: apdf.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/apdf-io/security/apdf-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- PDF
- Analytics
- API
- SaaS
- Engagement
---
