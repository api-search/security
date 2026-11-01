---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pace.group
  spf: false
hosts:
- host: pace.group
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pace Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pace, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Pace
provider_slug: pace-group
slug: pace-group-domain-security
source_filename: pace-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pace.group\n  https: false\ndomains:\n- domain: pace.group\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/pace-group/security/pace-group-domain-security.yml
summary_line: DMARC
tags:
- Company
---
