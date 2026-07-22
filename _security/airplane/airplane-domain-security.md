---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: airplane.dev
  spf: true
hosts:
- host: www.airplane.dev
  https: false
kind: domain-security
layout: security
method: probed
name: Airplane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airplane, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Airplane
provider_slug: airplane
slug: airplane-domain-security
source_filename: airplane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airplane.dev\n  https: false\ndomains:\n- domain: airplane.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airplane/refs/heads/main/security/airplane-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Developer Tools
- Internal Tools
- Workflows
- Automation
- Defunct
---
