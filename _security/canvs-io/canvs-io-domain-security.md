---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: canvs.io
  spf: true
hosts:
- cert_expires: Dec 18 15:59:29 2026 GMT
  host: canvs.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Canvs Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canvs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Canvs
provider_slug: canvs-io
slug: canvs-io-domain-security
source_filename: canvs-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: canvs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 15:59:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: canvs.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/canvs-io/security/canvs-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Whiteboard
- Artificial Intelligence
- Visual
- Productivity
---
