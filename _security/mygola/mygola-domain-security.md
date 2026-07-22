---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mygola.com
  spf: true
hosts:
- host: mygola.com
  https: false
kind: domain-security
layout: security
method: probed
name: Mygola Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyGola, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MyGola
provider_slug: mygola
slug: mygola-domain-security
source_filename: mygola-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mygola.com\n  https: false\ndomains:\n- domain: mygola.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mygola/refs/heads/main/security/mygola-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Travel
- Trip Planning
- Startup
---
