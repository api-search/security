---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zeet.co
  spf: true
hosts:
- host: zeet.co
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zeet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zeet, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zeet
provider_slug: zeet
slug: zeet-domain-security
source_filename: zeet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zeet.co\n  https: false\ndomains:\n- domain: zeet.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/zeet/security/zeet-domain-security.yml
summary_line: DMARC
tags:
- Company
- Cloud
- DevOps
- Automation
- Platform
---
