---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: highly.co
  spf: false
hosts:
- host: www.highly.co
  https: false
kind: domain-security
layout: security
method: probed
name: Highly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Highly, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Highly
provider_slug: highly
slug: highly-domain-security
source_filename: highly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.highly.co\n  https: false\ndomains:\n- domain: highly.co\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highly/refs/heads/main/security/highly-domain-security.yml
summary_line: DNSSEC
tags:
- Company
---
