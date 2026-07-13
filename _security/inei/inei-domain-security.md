---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gob.pe
  spf: false
hosts:
- host: iinei.inei.gob.pe
  https: false
kind: domain-security
layout: security
method: probed
name: Inei Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for INEI, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: INEI
provider_slug: inei
slug: inei-domain-security
source_filename: inei-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iinei.inei.gob.pe\n  https: false\ndomains:\n- domain: gob.pe\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inei/refs/heads/main/security/inei-domain-security.yml
summary_line: DNSSEC
tags:
- Government
- Public APIs
---
