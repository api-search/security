---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pusan.ac.kr
  spf: true
hosts:
- host: www.cse.pusan.ac.kr
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pusan National University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pusan National University, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pusan National University
provider_slug: pusan-national-university
slug: pusan-national-university-domain-security
source_filename: pusan-national-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cse.pusan.ac.kr\n  https: false\ndomains:\n- domain: pusan.ac.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/pusan-national-university/security/pusan-national-university-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
