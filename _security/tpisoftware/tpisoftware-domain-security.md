---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tpisoftware.com
  spf: false
hosts:
- host: tpisoftware.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tpisoftware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TPIsoftware, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: TPIsoftware
provider_slug: tpisoftware
slug: tpisoftware-domain-security
source_filename: tpisoftware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tpisoftware.com\n  https: false\ndomains:\n- domain: tpisoftware.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/tpisoftware/security/tpisoftware-domain-security.yml
summary_line: DMARC
tags:
- Company
- Fintech
- Open Banking
- Developer Tools
---
