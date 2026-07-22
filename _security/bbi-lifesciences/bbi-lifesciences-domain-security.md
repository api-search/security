---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bbi-lifesciences.com
  spf: true
hosts:
- host: bbi-lifesciences.com
  https: false
kind: domain-security
layout: security
method: probed
name: Bbi Lifesciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bbi-lifesciences, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: bbi-lifesciences
provider_slug: bbi-lifesciences
slug: bbi-lifesciences-domain-security
source_filename: bbi-lifesciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bbi-lifesciences.com\n  https: false\ndomains:\n- domain: bbi-lifesciences.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bbi-lifesciences/refs/heads/main/security/bbi-lifesciences-domain-security.yml
summary_line: DMARC
tags:
- Company
- Life Sciences
---
