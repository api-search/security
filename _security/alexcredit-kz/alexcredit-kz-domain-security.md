---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: alexcredit.kz
  spf: true
hosts:
- host: alexcredit.kz
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AlexCredit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AlexCredit, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AlexCredit
provider_slug: alexcredit-kz
slug: alexcredit-kz-domain-security
source_filename: alexcredit-kz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alexcredit.kz\n  https: false\ndomains:\n- domain: alexcredit.kz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/alexcredit-kz/security/alexcredit-kz-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Finance
- Kazakhstan
- Lending
- Microfinance
- Consumer
---
