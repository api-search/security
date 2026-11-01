---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: saicmotor.com
  spf: true
hosts:
- host: saicmotor.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Saic Motor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MG (SAIC Motor), probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MG (SAIC Motor)
provider_slug: saic-motor
slug: saic-motor-domain-security
source_filename: saic-motor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: saicmotor.com\n  https: false\ndomains:\n- domain: saicmotor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/saic-motor/security/saic-motor-domain-security.yml
summary_line: DMARC
tags:
- Company
- Automotive
- Manufacturing
- China
- MG
---
