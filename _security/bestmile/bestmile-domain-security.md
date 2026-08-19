---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bestmile.com
  spf: true
hosts:
- host: bestmile.com
  https: false
kind: domain-security
layout: security
method: probed
name: Bestmile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bestmile, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bestmile
provider_slug: bestmile
slug: bestmile-domain-security
source_filename: bestmile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bestmile.com\n  https: false\ndomains:\n- domain: bestmile.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bestmile/refs/heads/main/security/bestmile-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Applicative Saas
- Mobility
- Fleet Orchestration
- Autonomous Vehicles
- Transportation
- Mobility As A Service
---
