---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: paceup.com
  spf: true
hosts:
- host: paceup.com
  https: false
kind: domain-security
layout: security
method: probed
name: Pace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pace, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pace
provider_slug: pace
slug: pace-domain-security
source_filename: pace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paceup.com\n  https: false\ndomains:\n- domain: paceup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pace/refs/heads/main/security/pace-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Enterprise Software
---
