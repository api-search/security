---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: akaritx.com
  spf: true
hosts:
- host: www.akaritx.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Akari Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akari Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Akari Therapeutics
provider_slug: akari-therapeutics
slug: akari-therapeutics-domain-security
source_filename: akari-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.akaritx.com\n  https: false\ndomains:\n- domain: akaritx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/akari-therapeutics/security/akari-therapeutics-domain-security.yml
summary_line: DMARC
tags:
- Company
- Oncology
- ADC
- Biotechnology
- Therapeutics
- Clinical-Development
---
