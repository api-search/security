---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mmobomb.com
  spf: true
hosts:
- cert_expires: Sep  1 11:53:35 2026 GMT
  host: www.mmobomb.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mmo Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MMO Games, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MMO Games
provider_slug: mmo-games
slug: mmo-games-domain-security
source_filename: mmo-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mmobomb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 11:53:35 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: mmobomb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mmo-games/refs/heads/main/security/mmo-games-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Games And Comics
- Public APIs
---
