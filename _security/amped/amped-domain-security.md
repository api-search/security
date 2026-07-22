---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: applauze.com
  spf: true
hosts:
- host: applauze.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amped Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amped, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Amped
provider_slug: amped
slug: amped-domain-security
source_filename: amped-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: applauze.com\n  https: false\ndomains:\n- domain: applauze.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amped/refs/heads/main/security/amped-domain-security.yml
summary_line: DMARC
tags:
- Company
---
