---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deckodex.com
  spf: true
hosts:
- cert_expires: Jan 18 23:34:19 2027 GMT
  host: deckodex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deckodex Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deckodex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Deckodex
provider_slug: deckodex-com
slug: deckodex-com-domain-security
source_filename: deckodex-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deckodex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:34:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: deckodex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/deckodex-com/security/deckodex-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- deckbuilder
- Card Database
- collection tracking
- Trading Card Games
- Price-Tracking
- tournament meta
---
