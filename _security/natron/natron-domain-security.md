---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: natron.energy
  spf: true
hosts:
- host: natron.energy
  https: false
kind: domain-security
layout: security
method: probed
name: Natron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Natron Energy, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Natron Energy
provider_slug: natron
slug: natron-domain-security
source_filename: natron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: natron.energy\n  https: false\ndomains:\n- domain: natron.energy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natron/refs/heads/main/security/natron-domain-security.yml
summary_line: DMARC
tags:
- Energy Storage
- Batteries
- Sodium-Ion Batteries
- Prussian Blue Analog
- PBA Chemistry
- Data Center UPS
- Critical Power
- Industrial Backup
- Peak Shaving
- EV Charging Support
- Hardware
- Cleantech
- U.S. Manufacturing
- Defunct
---
