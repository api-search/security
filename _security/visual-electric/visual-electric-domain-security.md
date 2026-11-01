---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: visualelectric.com
  spf: true
hosts:
- host: visualelectric.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Visual Electric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Visual Electric, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Visual Electric
provider_slug: visual-electric
slug: visual-electric-domain-security
source_filename: visual-electric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: visualelectric.com\n  https: false\ndomains:\n- domain: visualelectric.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/visual-electric/security/visual-electric-domain-security.yml
summary_line: DMARC
tags:
- Company
---
