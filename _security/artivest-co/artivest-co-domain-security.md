---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: artivest.co
  spf: true
hosts:
- host: artivest.co
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Artivest Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artivest, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Artivest
provider_slug: artivest-co
slug: artivest-co-domain-security
source_filename: artivest-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: artivest.co\n  https: false\ndomains:\n- domain: artivest.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/artivest-co/security/artivest-co-domain-security.yml
summary_line: DMARC
tags:
- Company
- Investment
- Platform
- PrivateEquity
- RealEstate
- VentureCapital
---
