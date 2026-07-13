---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fusebit.io
  spf: true
hosts:
- host: fusebit.io
  https: false
kind: domain-security
layout: security
method: probed
name: Fusebit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fusebit, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fusebit
provider_slug: fusebit
slug: fusebit-domain-security
source_filename: fusebit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fusebit.io\n  https: false\ndomains:\n- domain: fusebit.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/security/fusebit-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Developer Tools
- Embedded iPaaS
- Integration
- Acquired
---
