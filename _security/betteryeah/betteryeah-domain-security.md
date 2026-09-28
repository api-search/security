---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: betteryeah.com
  spf: false
hosts:
- host: betteryeah.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Betteryeah Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Betteryeah, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Betteryeah
provider_slug: betteryeah
slug: betteryeah-domain-security
source_filename: betteryeah-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: betteryeah.com\n  https: false\ndomains:\n- domain: betteryeah.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betteryeah/refs/heads/main/security/betteryeah-domain-security.yml
summary_line: DNSSEC
tags:
- Company
---
