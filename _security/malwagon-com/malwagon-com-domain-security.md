---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: malwagon.com
  spf: true
hosts:
- host: malwagon.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: malwagon-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for malwagon-com, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: malwagon-com
provider_slug: malwagon-com
slug: malwagon-com-domain-security
source_filename: malwagon-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: malwagon.com\n  https: false\ndomains:\n- domain: malwagon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/malwagon-com/security/malwagon-com-domain-security.yml
summary_line: DMARC
tags:
- Company
---
