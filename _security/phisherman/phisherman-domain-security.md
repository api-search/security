---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: phisherman.gg
  spf: true
hosts:
- host: phisherman.gg
  https: false
kind: domain-security
layout: security
method: probed
name: Phisherman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phisherman, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Phisherman
provider_slug: phisherman
slug: phisherman-domain-security
source_filename: phisherman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: phisherman.gg\n  https: false\ndomains:\n- domain: phisherman.gg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phisherman/refs/heads/main/security/phisherman-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Anti Malware
- Public APIs
---
