---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: open-flux.fr
  spf: false
hosts:
- host: open-flux.fr
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Open Flux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MaSolutionDev, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: MaSolutionDev
provider_slug: open-flux
slug: open-flux-domain-security
source_filename: open-flux-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open-flux.fr\n  https: false\ndomains:\n- domain: open-flux.fr\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/open-flux/security/open-flux-domain-security.yml
summary_line: DNSSEC
tags:
- Company
---
