---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: marjory.io
  spf: true
hosts:
- host: marjory.io
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Marjory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marjory, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Marjory
provider_slug: marjory
slug: marjory-domain-security
source_filename: marjory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marjory.io\n  https: false\ndomains:\n- domain: marjory.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/marjory/security/marjory-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- SaaS
- Automation
- API
- Workflow
---
