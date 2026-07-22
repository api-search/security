---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: neotract.com
  spf: true
hosts:
- host: www.neotract.com
  https: false
kind: domain-security
layout: security
method: probed
name: Neotract Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NeoTract, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: NeoTract
provider_slug: neotract
slug: neotract-domain-security
source_filename: neotract-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neotract.com\n  https: false\ndomains:\n- domain: neotract.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neotract/refs/heads/main/security/neotract-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Medical Devices
- Health
- MedTech
- Medical
---
