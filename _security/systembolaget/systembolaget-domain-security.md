---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: systembolaget.se
  spf: true
hosts:
- host: api-portal.systembolaget.se
  https: false
kind: domain-security
layout: security
method: probed
name: Systembolaget Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Systembolaget, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Systembolaget
provider_slug: systembolaget
slug: systembolaget-domain-security
source_filename: systembolaget-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api-portal.systembolaget.se\n  https: false\ndomains:\n- domain: systembolaget.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/systembolaget/refs/heads/main/security/systembolaget-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Food And Drink
- Public APIs
---
