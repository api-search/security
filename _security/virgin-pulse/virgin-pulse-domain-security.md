---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: virginpulse.com
  spf: true
hosts:
- host: www.virginpulse.com
  https: false
kind: domain-security
layout: security
method: probed
name: Virgin Pulse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virgin Pulse, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Virgin Pulse
provider_slug: virgin-pulse
slug: virgin-pulse-domain-security
source_filename: virgin-pulse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.virginpulse.com\n  https: false\ndomains:\n- domain: virginpulse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virgin-pulse/refs/heads/main/security/virgin-pulse-domain-security.yml
summary_line: DMARC
tags:
- Company
- Healthcare
- Wellbeing
- Employee Wellness
- Health Navigation
- Benefits Administration
- Digital Health
- Personify Health
---
