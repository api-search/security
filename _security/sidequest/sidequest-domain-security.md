---
api_specs:
- filename: sidequest-openapi.json
  format: json
  label: SideQuest Public API
  slug: sidequest-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sidequest/refs/heads/main/openapi/sidequest-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sidequestvr.com
  spf: true
hosts:
- cert_expires: Oct  5 19:01:31 2026 GMT
  host: sidequestvr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 09:19:19 2026 GMT
  host: api.sidequestvr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sidequest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SideQuest, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SideQuest
provider_slug: sidequest
slug: sidequest-domain-security
source_filename: sidequest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sidequestvr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 19:01:31 2026 GMT\n  hsts: false\n- host: api.sidequestvr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 09:19:19 2026 GMT\n  hsts: null\ndomains:\n- domain: sidequestvr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sidequest/refs/heads/main/security/sidequest-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Virtual Reality
- VR
- XR
- Gaming
- App Store
- Developers
---
