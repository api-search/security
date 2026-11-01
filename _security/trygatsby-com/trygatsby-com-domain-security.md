---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trygatsby.com
  spf: true
hosts:
- host: trygatsby.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trygatsby Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gatsby, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Gatsby
provider_slug: trygatsby-com
slug: trygatsby-com-domain-security
source_filename: trygatsby-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trygatsby.com\n  https: false\ndomains:\n- domain: trygatsby.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/trygatsby-com/security/trygatsby-com-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
