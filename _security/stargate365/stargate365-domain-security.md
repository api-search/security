---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: stargate365.com
  spf: true
hosts:
- host: stargate365.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stargate365 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Surfstats software, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Surfstats software
provider_slug: stargate365
slug: stargate365-domain-security
source_filename: stargate365-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stargate365.com\n  https: false\ndomains:\n- domain: stargate365.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/stargate365/security/stargate365-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Analytics
- Data
- Surf
- API
---
