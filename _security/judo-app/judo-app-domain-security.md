---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: judo.app
  spf: true
hosts:
- host: judo.app
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Judo App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rover, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rover
provider_slug: judo-app
slug: judo-app-domain-security
source_filename: judo-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: judo.app\n  https: false\ndomains:\n- domain: judo.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/judo-app/security/judo-app-domain-security.yml
summary_line: DMARC
tags:
- Company
- No-code
- SwiftUI
- Mobile
- DeveloperTools
---
