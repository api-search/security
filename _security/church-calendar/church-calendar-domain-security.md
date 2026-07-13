---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: inadiutorium.cz
  spf: false
hosts:
- host: calapi.inadiutorium.cz
  https: false
kind: domain-security
layout: security
method: probed
name: Church Calendar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Church Calendar, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Church Calendar
provider_slug: church-calendar
slug: church-calendar-domain-security
source_filename: church-calendar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: calapi.inadiutorium.cz\n  https: false\ndomains:\n- domain: inadiutorium.cz\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/church-calendar/refs/heads/main/security/church-calendar-domain-security.yml
summary_line: DNSSEC
tags:
- Calendar
- Public APIs
---
