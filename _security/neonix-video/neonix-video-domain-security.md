---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: neonix.video
  spf: true
hosts:
- cert_expires: Jan 24 16:56:22 2027 GMT
  host: neonix.video
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Neonix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neonix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Neonix
provider_slug: neonix-video
slug: neonix-video-domain-security
source_filename: neonix-video-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neonix.video\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 16:56:22 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: neonix.video\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/neonix-video/security/neonix-video-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Video Editing
- Artificial Intelligence
- Desktop
- macOS
- iPhone
---
