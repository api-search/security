---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: strateos.com
  spf: true
hosts:
- host: strateos.com
  https: false
- host: developers.strateos.com
  https: false
- host: secure.strateos.com
  https: false
kind: domain-security
layout: security
method: probed
name: Strateos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Strateos, probed live across 3 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Strateos
provider_slug: strateos
slug: strateos-domain-security
source_filename: strateos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: strateos.com\n  https: false\n- host: developers.strateos.com\n  https: false\n- host: secure.strateos.com\n  https: false\ndomains:\n- domain: strateos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strateos/refs/heads/main/security/strateos-domain-security.yml
summary_line: DMARC
tags:
- Company
- Life Sciences
- Laboratory Automation
- Robotics
- Cloud Lab
- Drug Discovery
- Biotechnology
- Autoprotocol
- JSON:API
- Research
---
