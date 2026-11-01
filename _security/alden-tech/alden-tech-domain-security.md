---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alden.tech
  spf: true
hosts:
- host: alden.tech
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alden Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smart Diagnostics Systems, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Smart Diagnostics Systems
provider_slug: alden-tech
slug: alden-tech-domain-security
source_filename: alden-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alden.tech\n  https: false\ndomains:\n- domain: alden.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/alden-tech/security/alden-tech-domain-security.yml
summary_line: DMARC
tags:
- Company
- Diagnostics
- Microbiology
- Food Safety
- Healthcare
- API
---
