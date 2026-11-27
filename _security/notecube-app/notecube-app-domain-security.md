---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: notecube.app
  spf: false
hosts:
- cert_expires: Feb 16 09:27:56 2027 GMT
  host: notecube.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NoteCube Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NoteCube, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: NoteCube
provider_slug: notecube-app
slug: notecube-app-domain-security
source_filename: notecube-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: notecube.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 09:27:56 2027 GMT\n  hsts: false\ndomains:\n- domain: notecube.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/notecube-app/security/notecube-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Voice recorder
- Transcription
- Productivity
- Mobile App
---
