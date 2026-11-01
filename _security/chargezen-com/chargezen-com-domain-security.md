---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chargezen.com
  spf: true
hosts:
- host: chargezen.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chargezen Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for chargezen-com, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: chargezen-com
provider_slug: chargezen-com
slug: chargezen-com-domain-security
source_filename: chargezen-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chargezen.com\n  https: false\ndomains:\n- domain: chargezen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/chargezen-com/security/chargezen-com-domain-security.yml
summary_line: DMARC
tags:
- Company
---
