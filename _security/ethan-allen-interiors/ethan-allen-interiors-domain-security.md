---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ethanallen.com
  spf: true
hosts:
- cert_expires: Oct  3 19:16:00 2026 GMT
  host: www.ethanallen.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: developer.ethanallen.com
  https: false
- host: api.ethanallen.com
  https: false
kind: domain-security
layout: security
method: probed
name: Ethan Allen Interiors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ethan Allen Interiors, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ethan Allen Interiors
provider_slug: ethan-allen-interiors
slug: ethan-allen-interiors-domain-security
source_filename: ethan-allen-interiors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ethanallen.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 19:16:00 2026 GMT\n  hsts: false\n- host: developer.ethanallen.com\n  https: false\n- host: api.ethanallen.com\n  https: false\ndomains:\n- domain: ethanallen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ethan-allen-interiors/refs/heads/main/security/ethan-allen-interiors-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Furniture
- Home Design
- Retail
---
