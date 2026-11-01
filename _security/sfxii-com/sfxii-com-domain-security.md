---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sfxii.com
  spf: true
hosts:
- host: sfxii.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sfxii Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SFX, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SFX
provider_slug: sfxii-com
slug: sfxii-com-domain-security
source_filename: sfxii-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sfxii.com\n  https: false\ndomains:\n- domain: sfxii.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/sfxii-com/security/sfxii-com-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Fintech
- APIs
- Financial Services
- Developer Platform
---
