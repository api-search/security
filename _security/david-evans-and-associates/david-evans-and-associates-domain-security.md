---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: deainc.com
  spf: true
hosts:
- host: www.deainc.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: David Evans And Associates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for David Evans and Associates, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: David Evans and Associates
provider_slug: david-evans-and-associates
slug: david-evans-and-associates-domain-security
source_filename: david-evans-and-associates-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deainc.com\n  https: false\ndomains:\n- domain: deainc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/david-evans-and-associates/security/david-evans-and-associates-domain-security.yml
summary_line: DMARC
tags:
- Company
- Engineering
- Consulting
- Infrastructure
- Transportation
- Energy
---
