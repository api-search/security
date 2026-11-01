---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: nlsc.gov.tw
  spf: true
hosts:
- host: nlsc.gov.tw
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nlsc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NLSC (Taiwan), probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: NLSC (Taiwan)
provider_slug: nlsc
slug: nlsc-domain-security
source_filename: nlsc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nlsc.gov.tw\n  https: false\ndomains:\n- domain: nlsc.gov.tw\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nlsc/security/nlsc-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
---
