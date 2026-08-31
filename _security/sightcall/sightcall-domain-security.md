---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: sightcall.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: rtccloud.net
  spf: true
hosts:
- cert_expires: Oct 25 20:32:31 2026 GMT
  host: sightcall.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.rtccloud.net
  https: false
kind: domain-security
layout: security
method: probed
name: Sightcall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SightCall, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SightCall
provider_slug: sightcall
slug: sightcall-domain-security
source_filename: sightcall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sightcall.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 20:32:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rtccloud.net\n  https: false\ndomains:\n- domain: sightcall.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: rtccloud.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sightcall/refs/heads/main/security/sightcall-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Video
- WebRTC
- Remote Support
- Field Service
- Augmented Reality
- Computer-Vision
- Customer Service
- Insurance
- Telehealth
- Communications
---
