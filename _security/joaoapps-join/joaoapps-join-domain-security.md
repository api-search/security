---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: joaoapps.com
  spf: true
hosts:
- host: joaoapps.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Joaoapps Join Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Join and Tasker (joaoapps), probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Join and Tasker (joaoapps)
provider_slug: joaoapps-join
slug: joaoapps-join-domain-security
source_filename: joaoapps-join-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joaoapps.com\n  https: false\ndomains:\n- domain: joaoapps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/joaoapps-join/security/joaoapps-join-domain-security.yml
summary_line: DMARC
tags:
- Company
---
