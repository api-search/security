---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pylontech.com
  spf: true
hosts:
- host: pylontech.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pylontech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pylontech, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pylontech
provider_slug: pylontech
slug: pylontech-domain-security
source_filename: pylontech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pylontech.com\n  https: false\ndomains:\n- domain: pylontech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/pylontech/security/pylontech-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Energy
- Batteries
- Storage
- South Korea
---
