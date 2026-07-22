---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: slikpro.com
  spf: true
hosts:
- host: slikpro.com
  https: false
kind: domain-security
layout: security
method: probed
name: Slik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Slik, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Slik
provider_slug: slik
slug: slik-domain-security
source_filename: slik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: slikpro.com\n  https: false\ndomains:\n- domain: slikpro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slik/refs/heads/main/security/slik-domain-security.yml
summary_line: DMARC
tags:
- Company
- Employee Experience
- Employee Engagement
- Human Resources
- People Analytics
- Surveys
- Performance Management
- OKRs
- Employee Wellbeing
- SaaS
- Latin America
---
