---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mindmelt.de
  spf: true
hosts:
- host: mindmelt.de
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: mindmelt-de Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mindmelt-de, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: mindmelt-de
provider_slug: mindmelt-de
slug: mindmelt-de-domain-security
source_filename: mindmelt-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mindmelt.de\n  https: false\ndomains:\n- domain: mindmelt.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mindmelt-de/security/mindmelt-de-domain-security.yml
summary_line: DMARC
tags:
- Company
---
