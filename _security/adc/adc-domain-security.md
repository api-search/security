---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adc.com
  spf: true
hosts:
- host: adc.com
  https: false
kind: domain-security
layout: security
method: probed
name: Adc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adc, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Adc
provider_slug: adc
slug: adc-domain-security
source_filename: adc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adc.com\n  https: false\ndomains:\n- domain: adc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adc/refs/heads/main/security/adc-domain-security.yml
summary_line: DMARC
tags:
- Company
- Unknown
---
