---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: supplant.com
  spf: true
hosts:
- host: supplant.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: The Supplant Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Supplant Company, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Supplant Company
provider_slug: the-supplant-company
slug: the-supplant-company-domain-security
source_filename: the-supplant-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: supplant.com\n  https: false\ndomains:\n- domain: supplant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/the-supplant-company/security/the-supplant-company-domain-security.yml
summary_line: DMARC
tags:
- Company
---
