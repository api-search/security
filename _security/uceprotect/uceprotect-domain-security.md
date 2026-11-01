---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: uceprotect.net
  spf: true
hosts:
- host: uceprotect.net
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Uceprotect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UCEPROTECT, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: UCEPROTECT
provider_slug: uceprotect
slug: uceprotect-domain-security
source_filename: uceprotect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uceprotect.net\n  https: false\ndomains:\n- domain: uceprotect.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/uceprotect/security/uceprotect-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- SpamProtection
- EmailSecurity
- Blacklist
- NetworkSecurity
- Switzerland
---
