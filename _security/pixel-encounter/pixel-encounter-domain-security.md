---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pixelencounter.com
  spf: true
hosts:
- cert_expires: Aug 14 17:01:00 2026 GMT
  host: pixelencounter.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pixel Encounter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pixel Encounter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pixel Encounter
provider_slug: pixel-encounter
slug: pixel-encounter-domain-security
source_filename: pixel-encounter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pixelencounter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 17:01:00 2026 GMT\n  hsts: null\ndomains:\n- domain: pixelencounter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixel-encounter/refs/heads/main/security/pixel-encounter-domain-security.yml
summary_line: TLSv1.3
tags:
- Art And Design
- Public APIs
---
