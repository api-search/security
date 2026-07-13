---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: soketi.app
  spf: true
hosts:
- cert_expires: Sep 15 08:05:55 2026 GMT
  host: soketi.app
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 07:09:33 2026 GMT
  host: docs.soketi.app
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Soketi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soketi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Soketi
provider_slug: soketi
slug: soketi-domain-security
source_filename: soketi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: soketi.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 08:05:55 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: docs.soketi.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 07:09:33 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: soketi.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soketi/refs/heads/main/security/soketi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Realtime
- WebSockets
- Open Source
- Pusher Protocol
- Self-Host
- Drop-in
---
