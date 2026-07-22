---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: graybar-electric.com
  spf: false
hosts:
- host: www.graybar-electric.com
  https: false
kind: domain-security
layout: security
method: probed
name: Graybar Electric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for graybar-electric, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: graybar-electric
provider_slug: graybar-electric
slug: graybar-electric-domain-security
source_filename: graybar-electric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.graybar-electric.com\n  https: false\ndomains:\n- domain: graybar-electric.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graybar-electric/refs/heads/main/security/graybar-electric-domain-security.yml
summary_line: DMARC
tags:
- Fortune 500
---
