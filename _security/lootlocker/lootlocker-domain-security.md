---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lootlocker.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lootlocker.io
  spf: true
hosts:
- cert_expires: Aug 23 11:39:42 2026 GMT
  host: lootlocker.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 11:39:42 2026 GMT
  host: ref.lootlocker.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 20:32:49 2026 GMT
  host: api.lootlocker.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lootlocker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LootLocker, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: LootLocker
provider_slug: lootlocker
slug: lootlocker-domain-security
source_filename: lootlocker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lootlocker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 11:39:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ref.lootlocker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 11:39:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lootlocker.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 20:32:49 2026 GMT\n  hsts: null\ndomains:\n- domain: lootlocker.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: lootlocker.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lootlocker/refs/heads/main/security/lootlocker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Games
- Game Backend
- Game Backend as a Service
- Player Authentication
- Leaderboards
- Progressions
- Virtual Economy
- Cloud Save
- Cross-Platform
- Multiplayer
---
