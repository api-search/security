---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ondigo.me
  spf: true
hosts:
- host: ondigo.me
  https: false
kind: domain-security
layout: security
method: probed
name: Ondigo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ONDiGO, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ONDiGO
provider_slug: ondigo
slug: ondigo-domain-security
source_filename: ondigo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ondigo.me\n  https: false\ndomains:\n- domain: ondigo.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ondigo/refs/heads/main/security/ondigo-domain-security.yml
summary_line: DMARC
tags:
- Company
---
