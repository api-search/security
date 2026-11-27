---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cubite.io
  spf: true
hosts:
- host: cubite.io
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cubite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cubite, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cubite
provider_slug: cubite-io
slug: cubite-io-domain-security
source_filename: cubite-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cubite.io\n  https: false\ndomains:\n- domain: cubite.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cubite-io/security/cubite-io-domain-security.yml
summary_line: DMARC
tags:
- Company
- LMS
- Education
- EdTech
- E-Learning
- SCORM
- xAPI
- MCP
- Multi-Tenant
---
