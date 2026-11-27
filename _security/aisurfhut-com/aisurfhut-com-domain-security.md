---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aisurfhut.com
  spf: true
hosts:
- host: aisurfhut.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: aisurfhut-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aisurfhut-com, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: aisurfhut-com
provider_slug: aisurfhut-com
slug: aisurfhut-com-domain-security
source_filename: aisurfhut-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aisurfhut.com\n  https: false\ndomains:\n- domain: aisurfhut.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aisurfhut-com/security/aisurfhut-com-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
