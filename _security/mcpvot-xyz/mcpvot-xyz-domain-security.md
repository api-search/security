---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: mcpvot.xyz
  spf: true
hosts:
- host: mcpvot.xyz
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: mcpvot-xyz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mcpvot-xyz, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: mcpvot-xyz
provider_slug: mcpvot-xyz
slug: mcpvot-xyz-domain-security
source_filename: mcpvot-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcpvot.xyz\n  https: false\ndomains:\n- domain: mcpvot.xyz\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mcpvot-xyz/security/mcpvot-xyz-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
