---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coachup.com
  spf: true
hosts:
- host: coachup.com
  https: false
kind: domain-security
layout: security
method: probed
name: Coachup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coachup, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Coachup
provider_slug: coachup
slug: coachup-domain-security
source_filename: coachup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coachup.com\n  https: false\ndomains:\n- domain: coachup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coachup/refs/heads/main/security/coachup-domain-security.yml
summary_line: DMARC
tags:
- Company
- Sports
- Coaching
- Marketplace
- Fitness
- Training
- Athletics
- Two-Sided Marketplace
---
