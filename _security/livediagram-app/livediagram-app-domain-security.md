---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: livediagram.app
  spf: true
hosts:
- cert_expires: Jan 25 07:54:54 2027 GMT
  host: livediagram.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LiveDiagram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiveDiagram, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LiveDiagram
provider_slug: livediagram-app
slug: livediagram-app-domain-security
source_filename: livediagram-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: livediagram.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 07:54:54 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: livediagram.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/livediagram-app/security/livediagram-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Diagramming
- Collaboration
- Whiteboard
- Workshops
- Open Source
- Real-Time Editing
- Templates
---
