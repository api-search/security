---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: scientificgames.com
  spf: true
hosts:
- cert_expires: Aug 24 20:03:29 2026 GMT
  host: www.scientificgames.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scientific Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scientific Games, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Scientific Games
provider_slug: scientific-games
slug: scientific-games-domain-security
source_filename: scientific-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scientificgames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 20:03:29 2026 GMT\n  hsts: false\ndomains:\n- domain: scientificgames.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scientific-games/refs/heads/main/security/scientific-games-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Lottery
- Lottery Technology
- iLottery
- Instant Tickets
- Sports Betting
- Government Lottery
- Gaming Systems
- Retail Technology
---
