---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thoroughcare.net
  spf: true
hosts:
- host: thoroughcare.net
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ThoroughCare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThoroughCare, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ThoroughCare
provider_slug: thoroughcare
slug: thoroughcare-domain-security
source_filename: thoroughcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thoroughcare.net\n  https: false\ndomains:\n- domain: thoroughcare.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/thoroughcare/security/thoroughcare-domain-security.yml
summary_line: DMARC
tags:
- Company
---
