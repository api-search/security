---
description: ''
domains: []
hosts: []
kind: domain-security
layout: security
method: probed
name: Freshmenu Domain Security
name_suffix: Domain Security
overview: Domain security posture for Freshmenu, probed live across 0 host(s) and 0 registrable domain(s).
provider_name: Freshmenu
provider_slug: freshmenu
slug: freshmenu-domain-security
source_filename: freshmenu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: freshmenu.com (DNS + TLS + HTTP header probe)\nhost: https://www.freshmenu.com\nnotes: >-\n  FreshMenu runs a consumer food-ordering website fronted by Cloudflare. There is\n  no public API / developer program, so this probe covers the corporate/consumer\n  web domain only. Absence of a record below is honest, observed data — not a gap\n  in this file.\ntls:\n  present: true\n  issuer: \"Let's Encrypt (E8)\"\n  not_before: '2026-05-26'\n  not_after: '2026-08-24'\nhsts:\n  present: false\n  header: null\nedge:\n  cdn: cloudflare\ndnssec:\n  present: false\ncaa:\n  present: false\n  records: []\nspf:\n  present: true\n  record: \"v=spf1 include:_spf.google.com include:in-iwc-spf.icewarpcloud.in ~all\"\ndmarc:\n  present: true\n  policy: none\n  record: \"v=DMARC1; p=none;\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshmenu/refs/heads/main/security/freshmenu-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Food Delivery
- Food Technology
- Cloud Kitchen
- Restaurant
- Consumer
- India
---
