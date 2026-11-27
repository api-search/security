---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sigencloud.com
  spf: true
hosts:
- host: sigencloud.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sigenergy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sigenergy, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sigenergy
provider_slug: sigenergy
slug: sigenergy-domain-security
source_filename: sigenergy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sigencloud.com\n  https: false\ndomains:\n- domain: sigencloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/sigenergy/security/sigenergy-domain-security.yml
summary_line: DMARC
tags:
- Company
---
