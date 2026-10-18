---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alisports.com
  spf: true
hosts:
- host: alisports.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alisports Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alisports, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alisports
provider_slug: alisports
slug: alisports-domain-security
source_filename: alisports-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alisports.com\n  https: false\ndomains:\n- domain: alisports.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alisports/refs/heads/main/security/alisports-domain-security.yml
summary_line: DMARC
tags:
- Sports
- Technology
- Event Management
- Analytics
- Company
---
