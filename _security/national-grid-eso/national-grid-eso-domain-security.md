---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nationalgrideso.com
  spf: true
hosts:
- host: data.nationalgrideso.com
  https: false
kind: domain-security
layout: security
method: probed
name: National Grid Eso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Grid ESO, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: National Grid ESO
provider_slug: national-grid-eso
slug: national-grid-eso-domain-security
source_filename: national-grid-eso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.nationalgrideso.com\n  https: false\ndomains:\n- domain: nationalgrideso.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-grid-eso/refs/heads/main/security/national-grid-eso-domain-security.yml
summary_line: DMARC
tags:
- Environment
- Public APIs
---
