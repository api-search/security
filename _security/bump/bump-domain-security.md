---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bu.mp
  spf: true
hosts:
- host: bu.mp
  https: false
kind: domain-security
layout: security
method: probed
name: Bump Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bump, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bump
provider_slug: bump
slug: bump-domain-security
source_filename: bump-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bu.mp\n  https: false\ndomains:\n- domain: bu.mp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bump/refs/heads/main/security/bump-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Mobile
- File Sharing
- Data Transfer
- Proximity
- SDK
- Defunct
- Acquired
---
