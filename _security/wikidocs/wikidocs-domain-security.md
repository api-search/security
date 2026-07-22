---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wikidocs.io
  spf: true
hosts:
- host: wikidocs.io
  https: false
kind: domain-security
layout: security
method: probed
name: Wikidocs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wikidocs, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Wikidocs
provider_slug: wikidocs
slug: wikidocs-domain-security
source_filename: wikidocs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wikidocs.io\n  https: false\ndomains:\n- domain: wikidocs.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wikidocs/refs/heads/main/security/wikidocs-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Collaboration
- Real-Time
- Documentation
- Productivity
- Acquired
- SaaS
---
