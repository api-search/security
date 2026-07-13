---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rockstargames.com
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.rockstargames.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: signin.rockstargames.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: scapi.rockstargames.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rockstar Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rockstar Games, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rockstar Games
provider_slug: rockstar-games
slug: rockstar-games-domain-security
source_filename: rockstar-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rockstargames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: signin.rockstargames.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: null\n- host: scapi.rockstargames.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: rockstargames.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rockstar-games/refs/heads/main/security/rockstar-games-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gaming
- Entertainment
- Video Games
- Grand Theft Auto
- Red Dead Redemption
- Identity
- OAuth
---
