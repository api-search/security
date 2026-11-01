---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nabstract.io
  spf: true
hosts:
- host: nabstract.io
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nabstract Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nabstract.io, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: nabstract.io
provider_slug: nabstract
slug: nabstract-domain-security
source_filename: nabstract-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nabstract.io\n  https: false\ndomains:\n- domain: nabstract.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/nabstract/security/nabstract-domain-security.yml
summary_line: DMARC
tags:
- Company
- Data
- Integration
- Cloud
- Automation
---
