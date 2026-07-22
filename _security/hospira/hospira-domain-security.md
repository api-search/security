---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hospira.com
  spf: true
hosts:
- host: www.hospira.com
  https: false
kind: domain-security
layout: security
method: probed
name: Hospira Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hospira, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hospira
provider_slug: hospira
slug: hospira-domain-security
source_filename: hospira-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hospira.com\n  https: false\ndomains:\n- domain: hospira.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hospira/refs/heads/main/security/hospira-domain-security.yml
summary_line: DMARC
tags:
- Healthcare
- Pharmaceuticals
- Medical Devices
---
