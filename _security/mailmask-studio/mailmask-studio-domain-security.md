---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mailmask.studio
  spf: true
hosts:
- host: mailmask.studio
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: mailmask-studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mailmask-studio, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: mailmask-studio
provider_slug: mailmask-studio
slug: mailmask-studio-domain-security
source_filename: mailmask-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailmask.studio\n  https: false\ndomains:\n- domain: mailmask.studio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mailmask-studio/security/mailmask-studio-domain-security.yml
summary_line: DMARC
tags:
- Company
---
