---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ourhealthmate.com
  spf: true
hosts:
- host: corporate.ourhealthmate.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ourhealthmate Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OurHealthMate, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OurHealthMate
provider_slug: ourhealthmate-com
slug: ourhealthmate-com-domain-security
source_filename: ourhealthmate-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corporate.ourhealthmate.com\n  https: false\ndomains:\n- domain: ourhealthmate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ourhealthmate-com/security/ourhealthmate-com-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
