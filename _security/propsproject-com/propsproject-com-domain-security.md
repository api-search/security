---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: propsproject.com
  spf: true
hosts:
- host: propsproject.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Propsproject Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Props, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Props
provider_slug: propsproject-com
slug: propsproject-com-domain-security
source_filename: propsproject-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: propsproject.com\n  https: false\ndomains:\n- domain: propsproject.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/propsproject-com/security/propsproject-com-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Asset Management
- API
- Startup
- Inventory
- Developer Friendly
---
