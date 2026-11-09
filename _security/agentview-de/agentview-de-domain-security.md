---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentview.de
  spf: true
hosts:
- host: agentview.de
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentview De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for agentView, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: agentView
provider_slug: agentview-de
slug: agentview-de-domain-security
source_filename: agentview-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentview.de\n  https: false\ndomains:\n- domain: agentview.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agentview-de/security/agentview-de-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Artificial Intelligence
- Digital Signage
- GDPR
- Cloud
---
