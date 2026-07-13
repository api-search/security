---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tldraw.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: tldraw.dev
  spf: false
hosts:
- cert_expires: Sep 28 16:57:02 2026 GMT
  host: www.tldraw.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 03:16:21 2026 GMT
  host: tldraw.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tldraw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tldraw, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: tldraw
provider_slug: tldraw
slug: tldraw-domain-security
source_filename: tldraw-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tldraw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 16:57:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: tldraw.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 03:16:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tldraw.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tldraw.dev\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tldraw/refs/heads/main/security/tldraw-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Whiteboard
- SDK
- Canvas
- React
- Multiplayer
---
