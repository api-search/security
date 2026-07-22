---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tsumobi.com
  spf: true
hosts:
- host: tsumobi.com
  https: false
kind: domain-security
layout: security
method: probed
name: Tsumobi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tsumobi, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tsumobi
provider_slug: tsumobi
slug: tsumobi-domain-security
source_filename: tsumobi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tsumobi.com\n  https: false\ndomains:\n- domain: tsumobi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tsumobi/refs/heads/main/security/tsumobi-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Messaging
- Mobile
- J2ME
- Feature Phones
- Y Combinator
- Defunct
---
