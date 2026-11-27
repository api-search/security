---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: motiontext.video
  spf: false
hosts:
- cert_expires: Feb  7 21:44:23 2027 GMT
  host: motiontext.video
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Motion Text Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Motion Text, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Motion Text
provider_slug: motiontext-video
slug: motiontext-video-domain-security
source_filename: motiontext-video-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: motiontext.video\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 21:44:23 2027 GMT\n  hsts: false\ndomains:\n- domain: motiontext.video\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/motiontext-video/security/motiontext-video-domain-security.yml
summary_line: TLSv1.3
tags:
- Video Maker
- Static Assets
- Caption Sync
- Creators
- Indie Studios
- Product Teams
---
