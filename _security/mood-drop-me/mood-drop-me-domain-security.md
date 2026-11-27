---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mood-drop.me
  spf: true
hosts:
- cert_expires: Jan  8 23:28:53 2027 GMT
  host: mood-drop.me
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Last Drop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Last Drop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Last Drop
provider_slug: mood-drop-me
slug: mood-drop-me-domain-security
source_filename: mood-drop-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mood-drop.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:28:53 2027 GMT\n  hsts: false\ndomains:\n- domain: mood-drop.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mood-drop-me/security/mood-drop-me-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Game
- Web
- Multiplayer
- Free
---
