---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ghosty.studio
  spf: true
hosts:
- host: ghosty.studio
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ghosty Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ghosty-studio, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ghosty-studio
provider_slug: ghosty-studio
slug: ghosty-studio-domain-security
source_filename: ghosty-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ghosty.studio\n  https: false\ndomains:\n- domain: ghosty.studio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ghosty-studio/security/ghosty-studio-domain-security.yml
summary_line: DMARC
tags:
- Company
---
