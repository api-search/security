---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: polyxlabs.com
  spf: true
hosts:
- cert_expires: Jan 18 12:37:18 2027 GMT
  host: polyxlabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polyxlabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PolyXLabs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PolyXLabs
provider_slug: polyxlabs
slug: polyxlabs-domain-security
source_filename: polyxlabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: polyxlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 12:37:18 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: polyxlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polyxlabs/refs/heads/main/security/polyxlabs-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Sustainable Materials
- Biodegradable Plastics
- Sustainability
- Packaging
- Green Chemistry
---
