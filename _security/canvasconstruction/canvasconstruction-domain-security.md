---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: canvasbuilding.com
  spf: true
hosts:
- cert_expires: Nov 29 13:21:05 2026 GMT
  host: canvasbuilding.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Canvasconstruction Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canvasconstruction, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Canvasconstruction
provider_slug: canvasconstruction
slug: canvasconstruction-domain-security
source_filename: canvasconstruction-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: canvasbuilding.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 13:21:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: canvasbuilding.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canvasconstruction/refs/heads/main/security/canvasconstruction-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Construction
- Infrastructure
- Real Estate
- Engineering
---
