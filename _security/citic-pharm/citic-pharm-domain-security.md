---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: citic-pharm.com
  spf: true
hosts:
- host: citic-pharm.com
  https: false
kind: domain-security
layout: security
method: probed
name: Citic Pharm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for citic-pharm, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: citic-pharm
provider_slug: citic-pharm
slug: citic-pharm-domain-security
source_filename: citic-pharm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: citic-pharm.com\n  https: false\ndomains:\n- domain: citic-pharm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citic-pharm/refs/heads/main/security/citic-pharm-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
