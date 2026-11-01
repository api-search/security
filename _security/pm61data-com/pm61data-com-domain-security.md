---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pm61data.com
  spf: true
hosts:
- host: www.pm61data.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pm61Data Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Promethium, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Promethium
provider_slug: pm61data-com
slug: pm61data-com-domain-security
source_filename: pm61data-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pm61data.com\n  https: false\ndomains:\n- domain: pm61data.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/pm61data-com/security/pm61data-com-domain-security.yml
summary_line: DMARC
tags:
- Company
---
