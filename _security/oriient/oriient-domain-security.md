---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oriient.me
  spf: true
hosts:
- cert_expires: Aug 23 11:24:09 2026 GMT
  host: oriient.me
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Oriient Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oriient, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Oriient
provider_slug: oriient
slug: oriient-domain-security
source_filename: oriient-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oriient.me\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 23 11:24:09 2026 GMT\n  hsts: false\ndomains:\n- domain: oriient.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oriient/refs/heads/main/security/oriient-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Indoor Positioning
- Indoor Navigation
- Location Services
- Geolocation
- SDK
- Retail
- Asset Tracking
---
