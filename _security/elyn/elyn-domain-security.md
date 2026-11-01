---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: elyn.io
  spf: true
hosts:
- host: www.elyn.io
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Elyn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elyn, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Elyn
provider_slug: elyn
slug: elyn-domain-security
source_filename: elyn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elyn.io\n  https: false\ndomains:\n- domain: elyn.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/elyn/security/elyn-domain-security.yml
summary_line: DMARC
tags:
- Company
- Fintech
- APIs
- Compliance
- DataAnalytics
---
