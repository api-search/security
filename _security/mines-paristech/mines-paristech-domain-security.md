---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: mines-paristech.eu
  spf: true
hosts:
- host: www.mines-paristech.eu
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mines Paristech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MINES ParisTech, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MINES ParisTech
provider_slug: mines-paristech
slug: mines-paristech-domain-security
source_filename: mines-paristech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mines-paristech.eu\n  https: false\ndomains:\n- domain: mines-paristech.eu\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mines-paristech/security/mines-paristech-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
