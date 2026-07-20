---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: klang-games.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: seed.game
  spf: true
hosts:
- cert_expires: Sep 15 02:58:46 2026 GMT
  host: www.klang-games.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 21:25:26 2026 GMT
  host: seed.game
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 01:40:34 2026 GMT
  host: login.seed.game
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Klang Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klang Games, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Klang Games
provider_slug: klang
slug: klang-domain-security
source_filename: klang-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.klang-games.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:58:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: seed.game\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:25:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: login.seed.game\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 01:40:34 2026 GMT\n  hsts: false\ndomains:\n- domain: klang-games.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: seed.game\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klang/refs/heads/main/security/klang-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- Gaming
- Game Development
- MMO
- Simulation
- Entertainment
- Identity
- OpenID Connect
- Berlin
---
