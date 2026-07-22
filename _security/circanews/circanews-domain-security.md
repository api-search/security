---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: circanews.com
  spf: true
hosts:
- host: circanews.com
  https: false
kind: domain-security
layout: security
method: probed
name: Circanews Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for circanews, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: circanews
provider_slug: circanews
slug: circanews-domain-security
source_filename: circanews-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: circanews.com\n  https: false\ndomains:\n- domain: circanews.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circanews/refs/heads/main/security/circanews-domain-security.yml
summary_line: DMARC
tags:
- Company
---
