---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eqlgames.com
  spf: true
hosts:
- cert_expires: Mar 10 16:27:01 2027 GMT
  host: www.eqlgames.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eql Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EQL Games, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EQL Games
provider_slug: eql-games
slug: eql-games-domain-security
source_filename: eql-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eqlgames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 16:27:01 2027 GMT\n  hsts: false\ndomains:\n- domain: eqlgames.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eql-games/refs/heads/main/security/eql-games-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Lottery
- iLottery
- iGaming
- Games
- Game Studio
- Content Aggregator
- Licensing
- Entertainment
---
