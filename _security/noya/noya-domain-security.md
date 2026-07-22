---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: noya.co
  spf: true
hosts:
- host: www.noya.co
  https: false
kind: domain-security
layout: security
method: probed
name: Noya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noya, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Noya
provider_slug: noya
slug: noya-domain-security
source_filename: noya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.noya.co\n  https: false\ndomains:\n- domain: noya.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noya/refs/heads/main/security/noya-domain-security.yml
summary_line: DMARC
tags:
- Company
---
