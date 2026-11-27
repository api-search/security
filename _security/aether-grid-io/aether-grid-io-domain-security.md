---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aether-grid.io
  spf: true
hosts:
- cert_expires: Jan  6 10:01:10 2027 GMT
  host: aether-grid.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AETHER Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AETHER, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AETHER
provider_slug: aether-grid-io
slug: aether-grid-io-domain-security
source_filename: aether-grid-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aether-grid.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 10:01:10 2027 GMT\n  hsts: false\ndomains:\n- domain: aether-grid.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aether-grid-io/security/aether-grid-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- IoT
- Predictive Analytics
- Industrial
- Diagnostics
---
