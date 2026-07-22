---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: spitfireathlete.com
  spf: true
hosts:
- host: spitfireathlete.com
  https: false
kind: domain-security
layout: security
method: probed
name: Spitfire Athlete Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spitfire Athlete, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Spitfire Athlete
provider_slug: spitfire-athlete
slug: spitfire-athlete-domain-security
source_filename: spitfire-athlete-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spitfireathlete.com\n  https: false\ndomains:\n- domain: spitfireathlete.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spitfire-athlete/refs/heads/main/security/spitfire-athlete-domain-security.yml
summary_line: DNSSEC
tags:
- Company
---
