---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dte-energy.com
  spf: true
hosts:
- host: www.dte-energy.com
  https: false
kind: domain-security
layout: security
method: probed
name: Dte Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dte-energy, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: dte-energy
provider_slug: dte-energy
slug: dte-energy-domain-security
source_filename: dte-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dte-energy.com\n  https: false\ndomains:\n- domain: dte-energy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dte-energy/refs/heads/main/security/dte-energy-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Fortune 500
---
