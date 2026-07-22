---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: visor.io
  spf: true
hosts:
- host: visor.io
  https: false
kind: domain-security
layout: security
method: probed
name: Visor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Visor, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Visor
provider_slug: visor
slug: visor-domain-security
source_filename: visor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: visor.io\n  https: false\ndomains:\n- domain: visor.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visor/refs/heads/main/security/visor-domain-security.yml
summary_line: DMARC
tags:
- Company
---
