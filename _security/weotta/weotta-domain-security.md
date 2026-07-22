---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: weotta.com
  spf: true
hosts:
- host: weotta.com
  https: false
kind: domain-security
layout: security
method: probed
name: Weotta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for weotta, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: weotta
provider_slug: weotta
slug: weotta-domain-security
source_filename: weotta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: weotta.com\n  https: false\ndomains:\n- domain: weotta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weotta/refs/heads/main/security/weotta-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
