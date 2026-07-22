---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: caraway.health
  spf: true
hosts:
- host: caraway.health
  https: false
kind: domain-security
layout: security
method: probed
name: Caraway Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caraway Health *, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Caraway Health *
provider_slug: caraway-health
slug: caraway-health-domain-security
source_filename: caraway-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caraway.health\n  https: false\ndomains:\n- domain: caraway.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caraway-health/refs/heads/main/security/caraway-health-domain-security.yml
summary_line: DMARC
tags:
- Company
- Life Sciences
- Digital Health
- Telehealth
- Mental Health
- Healthcare
- Students
---
