---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 24haowan.com
  spf: true
hosts:
- host: 24haowan.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 24Haowan Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 24haowan-com, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 24haowan-com
provider_slug: 24haowan-com
slug: 24haowan-com-domain-security
source_filename: 24haowan-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 24haowan.com\n  https: false\ndomains:\n- domain: 24haowan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/24haowan-com/security/24haowan-com-domain-security.yml
summary_line: DMARC
tags:
- Company
---
