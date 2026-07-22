---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aus.co.in
  spf: true
hosts:
- host: aus.co.in
  https: false
kind: domain-security
layout: security
method: probed
name: Aus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AUS, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AUS
provider_slug: aus
slug: aus-domain-security
source_filename: aus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aus.co.in\n  https: false\ndomains:\n- domain: aus.co.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aus/refs/heads/main/security/aus-domain-security.yml
summary_line: DMARC
tags:
- Company
---
