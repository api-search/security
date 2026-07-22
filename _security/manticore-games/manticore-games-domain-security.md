---
description: ''
domains:
- caa:
  - 0 iodef "mailto:it@manticoregames.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: manticoregames.com
  spf: true
- caa:
  - 0 iodef "mailto:it@manticoregames.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coregames.com
  spf: true
hosts:
- cert_expires: Sep  2 21:23:50 2026 GMT
  host: www.manticoregames.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 08:23:48 2026 GMT
  host: docs.coregames.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Manticore Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Manticore Games, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Manticore Games
provider_slug: manticore-games
slug: manticore-games-domain-security
source_filename: manticore-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.manticoregames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 21:23:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.coregames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 08:23:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: manticoregames.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:it@manticoregames.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: coregames.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:it@manticoregames.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manticore-games/refs/heads/main/security/manticore-games-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Gaming
- Game Development
- Metaverse
- Creator Platform
- Lua
- Scripting
---
