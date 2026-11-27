---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: govideo.stream
  spf: true
hosts:
- cert_expires: Jan 27 13:30:42 2027 GMT
  host: govideo.stream
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GoVideo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoVideo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GoVideo
provider_slug: govideo-stream
slug: govideo-stream-domain-security
source_filename: govideo-stream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: govideo.stream\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 13:30:42 2027 GMT\n  hsts: false\ndomains:\n- domain: govideo.stream\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/govideo-stream/security/govideo-stream-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Video
- Streaming
- Hosting
- Media
- Platform
---
