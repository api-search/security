---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: saasler.com
  spf: true
hosts:
- host: saasler.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Saasler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koombea, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Koombea
provider_slug: saasler
slug: saasler-domain-security
source_filename: saasler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: saasler.com\n  https: false\ndomains:\n- domain: saasler.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/saasler/security/saasler-domain-security.yml
summary_line: DMARC
tags:
- Software-as-a-Service
- Automation
- Integration
- Marketing
- Sales
- Company
---
