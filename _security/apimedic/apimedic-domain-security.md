---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apimedic.com
  spf: true
hosts:
- host: apimedic.com
  https: false
kind: domain-security
layout: security
method: probed
name: Apimedic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ApiMedic, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ApiMedic
provider_slug: apimedic
slug: apimedic-domain-security
source_filename: apimedic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apimedic.com\n  https: false\ndomains:\n- domain: apimedic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apimedic/refs/heads/main/security/apimedic-domain-security.yml
summary_line: DMARC
tags:
- Sports And Fitness
- Public APIs
---
