---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: houmo.ai
  spf: true
hosts:
- host: houmo.ai
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Houmo Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for houmo, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: houmo
provider_slug: houmo-ai
slug: houmo-ai-domain-security
source_filename: houmo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: houmo.ai\n  https: false\ndomains:\n- domain: houmo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/houmo-ai/security/houmo-ai-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
