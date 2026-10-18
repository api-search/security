---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cognosos.com
  spf: true
hosts:
- host: cognosos.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cognosos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognosos, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cognosos
provider_slug: cognosos
slug: cognosos-domain-security
source_filename: cognosos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cognosos.com\n  https: false\ndomains:\n- domain: cognosos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognosos/refs/heads/main/security/cognosos-domain-security.yml
summary_line: DMARC
tags:
- Company
- Artificial Intelligence
- Location Intelligence
- Asset Tracking
- Healthcare
- Automotive
- Logistics
---
