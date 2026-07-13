---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: decathlon.com
  spf: true
hosts:
- host: developers.decathlon.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sport List And Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sport List & Data, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sport List & Data
provider_slug: sport-list-and-data
slug: sport-list-and-data-domain-security
source_filename: sport-list-and-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.decathlon.com\n  https: false\ndomains:\n- domain: decathlon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sport-list-and-data/refs/heads/main/security/sport-list-and-data-domain-security.yml
summary_line: DMARC
tags:
- Sports And Fitness
- Public APIs
---
