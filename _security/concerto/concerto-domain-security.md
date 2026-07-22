---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: concertocard.com
  spf: true
hosts:
- host: concertocard.com
  https: false
kind: domain-security
layout: security
method: probed
name: Concerto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Concerto, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Concerto
provider_slug: concerto
slug: concerto-domain-security
source_filename: concerto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: concertocard.com\n  https: false\ndomains:\n- domain: concertocard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/concerto/refs/heads/main/security/concerto-domain-security.yml
summary_line: DMARC
tags:
- Company
- Fintech
- Credit Cards
- Payments
- Cards
- Financial Services
---
