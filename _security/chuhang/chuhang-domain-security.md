---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chuhang.tech
  spf: true
hosts:
- host: chuhang.tech
  https: false
kind: domain-security
layout: security
method: probed
name: Chuhang Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for chuhang, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: chuhang
provider_slug: chuhang
slug: chuhang-domain-security
source_filename: chuhang-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chuhang.tech\n  https: false\ndomains:\n- domain: chuhang.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chuhang/refs/heads/main/security/chuhang-domain-security.yml
summary_line: DMARC
tags:
- Company
---
