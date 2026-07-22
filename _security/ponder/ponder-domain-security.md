---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ponder.io
  spf: true
hosts:
- host: ponder.io
  https: false
kind: domain-security
layout: security
method: probed
name: Ponder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ponder, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ponder
provider_slug: ponder
slug: ponder-domain-security
source_filename: ponder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ponder.io\n  https: false\ndomains:\n- domain: ponder.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ponder/refs/heads/main/security/ponder-domain-security.yml
summary_line: DMARC
tags:
- Company
- Data Science
- DataFrames
- Analytics
- Python
- Machine Learning
- Open Source
---
