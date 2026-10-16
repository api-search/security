---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: catayabio.com
  spf: true
hosts:
- host: catayabio.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Catayabio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Catayabio, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Catayabio
provider_slug: catayabio
slug: catayabio-domain-security
source_filename: catayabio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: catayabio.com\n  https: false\ndomains:\n- domain: catayabio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catayabio/refs/heads/main/security/catayabio-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Biotechnology
- Sustainable
- Ingredients
- Shanghai
- Personal Care
---
