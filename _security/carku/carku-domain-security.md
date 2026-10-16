---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: carku.com
  spf: true
hosts:
- host: www.carku.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carku, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Carku
provider_slug: carku
slug: carku-domain-security
source_filename: carku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carku.com\n  https: false\ndomains:\n- domain: carku.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carku/refs/heads/main/security/carku-domain-security.yml
summary_line: DMARC
tags:
- Automotive
- Energy
- Hardware
- Battery
- Shenzhen
---
