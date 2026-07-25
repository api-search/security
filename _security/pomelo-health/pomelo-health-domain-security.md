---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pomelohealth.com
  spf: true
hosts:
- host: www.pomelohealth.com
  https: false
kind: domain-security
layout: security
method: probed
name: Pomelo Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pomelo Health, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pomelo Health
provider_slug: pomelo-health
slug: pomelo-health-domain-security
source_filename: pomelo-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pomelohealth.com\n  https: false\ndomains:\n- domain: pomelohealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pomelo-health/refs/heads/main/security/pomelo-health-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Healthcare
- Canada
- Patient Engagement
- Telehealth
- Appointment Scheduling
- Patient Portal
- eForms
- EMR Integration
- TELUS Health
- Digital Health
---
