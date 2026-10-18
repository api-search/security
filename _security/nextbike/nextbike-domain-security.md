---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nextbike.net
  spf: true
hosts:
- host: www.nextbike.net
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nextbike Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nextbike, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: nextbike
provider_slug: nextbike
slug: nextbike-domain-security
source_filename: nextbike-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nextbike.net\n  https: false\ndomains:\n- domain: nextbike.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextbike/refs/heads/main/security/nextbike-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- BikeSharing
- Mobility
- Transportation
- Europe
- Software-as-a-Service
- Company
---
