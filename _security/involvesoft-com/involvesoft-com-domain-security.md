---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: involvesoft.com
  spf: true
hosts:
- host: involvesoft.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Involvesoft Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Involve.AI, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Involve.AI
provider_slug: involvesoft-com
slug: involvesoft-com-domain-security
source_filename: involvesoft-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: involvesoft.com\n  https: false\ndomains:\n- domain: involvesoft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/involvesoft-com/security/involvesoft-com-domain-security.yml
summary_line: DMARC
tags:
- Company
---
