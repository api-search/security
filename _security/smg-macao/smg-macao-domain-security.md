---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: smg.gov.mo
  spf: true
hosts:
- host: smg.gov.mo
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Smg Macao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SMG (Macao), probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SMG (Macao)
provider_slug: smg-macao
slug: smg-macao-domain-security
source_filename: smg-macao-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smg.gov.mo\n  https: false\ndomains:\n- domain: smg.gov.mo\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/smg-macao/security/smg-macao-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
