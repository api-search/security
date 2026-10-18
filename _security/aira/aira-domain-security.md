---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aira.com
  spf: true
hosts:
- host: aira.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aira Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aira, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aira
provider_slug: aira
slug: aira-domain-security
source_filename: aira-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aira.com\n  https: false\ndomains:\n- domain: aira.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aira/refs/heads/main/security/aira-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Accessibility
- VideoRemoteInterpreting
- AssistiveTechnology
- Software-as-a-Service
---
