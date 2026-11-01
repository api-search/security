---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fysical.com
  spf: true
hosts:
- host: fysical.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fysical Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paedae, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Paedae
provider_slug: fysical-com
slug: fysical-com-domain-security
source_filename: fysical-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fysical.com\n  https: false\ndomains:\n- domain: fysical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fysical-com/security/fysical-com-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
