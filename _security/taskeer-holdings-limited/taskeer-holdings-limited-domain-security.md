---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: taskeer.co
  spf: true
hosts:
- host: taskeer.co
  https: false
kind: domain-security
layout: security
method: probed
name: Taskeer Holdings Limited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taskeer Holdings Limited, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Taskeer Holdings Limited
provider_slug: taskeer-holdings-limited
slug: taskeer-holdings-limited-domain-security
source_filename: taskeer-holdings-limited-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taskeer.co\n  https: false\ndomains:\n- domain: taskeer.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taskeer-holdings-limited/refs/heads/main/security/taskeer-holdings-limited-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
