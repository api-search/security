---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: daikin.com
  spf: true
hosts:
- host: daikin.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Daikin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daikin, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Daikin
provider_slug: daikin
slug: daikin-domain-security
source_filename: daikin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: daikin.com\n  https: false\ndomains:\n- domain: daikin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/daikin/security/daikin-domain-security.yml
summary_line: DMARC
tags:
- Company
- HVAC
- Air-Conditioning
- Refrigeration
- Climate-Control
- Manufacturing
---
