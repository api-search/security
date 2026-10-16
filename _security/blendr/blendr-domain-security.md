---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blendr.io
  spf: true
hosts:
- host: blendr.io
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blendr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blendr.io, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blendr.io
provider_slug: blendr
slug: blendr-domain-security
source_filename: blendr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blendr.io\n  https: false\ndomains:\n- domain: blendr.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blendr/refs/heads/main/security/blendr-domain-security.yml
summary_line: DMARC
tags:
- Integration
- Automation
- API
- Workflow
- SaaS
- Data
---
