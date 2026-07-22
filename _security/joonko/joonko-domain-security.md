---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: joonko.co
  spf: true
hosts:
- host: joonko.co
  https: false
kind: domain-security
layout: security
method: probed
name: Joonko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for joonko, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: joonko
provider_slug: joonko
slug: joonko-domain-security
source_filename: joonko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joonko.co\n  https: false\ndomains:\n- domain: joonko.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/joonko/refs/heads/main/security/joonko-domain-security.yml
summary_line: DMARC
tags:
- Company
---
