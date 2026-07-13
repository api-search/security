---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: colourlovers.com
  spf: true
hosts:
- cert_expires: Oct  7 09:25:47 2026 GMT
  host: www.colourlovers.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Colourlovers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ColourLovers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ColourLovers
provider_slug: colourlovers
slug: colourlovers-domain-security
source_filename: colourlovers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.colourlovers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 09:25:47 2026 GMT\n  hsts: null\ndomains:\n- domain: colourlovers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colourlovers/refs/heads/main/security/colourlovers-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Art And Design
- Public APIs
---
