---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lily.camera
  spf: false
hosts:
- cert_expires: Sep 20 22:32:44 2026 GMT
  host: lily.camera
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lily Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lily Camera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Lily Camera
provider_slug: lily
slug: lily-domain-security
source_filename: lily-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lily.camera\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 22:32:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lily.camera\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lily/refs/heads/main/security/lily-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Drones
- Aerial Photography
- Videography
- Photography
- Marketplace
---
