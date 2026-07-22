---
description: ''
domains:
- caa: []
  dmarc: false
  dns_status: NXDOMAIN
  dnssec: false
  domain: stickies.wtf
  resolves: false
  spf: false
hosts:
- error: DNS NXDOMAIN — connection impossible
  host: stickies.wtf
  https: false
- error: DNS NXDOMAIN — connection impossible
  host: www.stickies.wtf
  https: false
kind: domain-security
layout: security
method: probed
name: Stickies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stickies, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Stickies
provider_slug: stickies
slug: stickies-domain-security
source_filename: stickies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nnote: >-\n  The company's only known domain, stickies.wtf, no longer resolves — every DNS\n  query (A, AAAA, NS, MX, TXT, CAA, DNSKEY, _dmarc, www) returns NXDOMAIN from\n  the .wtf zone, and HTTPS connections fail. The 0-working/probe-domain-security.py\n  probe reported the host unreachable and declined to write; this file records the\n  manual dig/curl observations. Wayback Machine shows the site last live 2023-03-11,\n  returning 403 by 2024-08, confirming the company appears defunct.\nhosts:\n- host: stickies.wtf\n  https: false\n  error: DNS NXDOMAIN — connection impossible\n- host: www.stickies.wtf\n  https: false\n  error: DNS NXDOMAIN — connection impossible\ndomains:\n- domain: stickies.wtf\n  resolves: false\n  dns_status: NXDOMAIN\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\nevidence:\n- 'dig SOA stickies.wtf -> status: NXDOMAIN (authority: wtf. zone SOA, 2026-07-21)'\n- 'dig A/AAAA/NS/MX/TXT/CAA/DNSKEY stickies.wtf\
  \ -> NXDOMAIN (2026-07-21)'\n- 'curl https://stickies.wtf and https://www.stickies.wtf -> exit 000, no connection (2026-07-21)'\n- 'web.archive.org: last 200 capture 2023-03-11; 403 by 2024-08-09'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stickies/refs/heads/main/security/stickies-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- NFT
- Web3
- Stickers
- GIFs
- Avatars
- Messaging
- Consumer
---
