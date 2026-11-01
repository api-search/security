---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: omie.es
  spf: true
hosts:
- host: omie.es
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Omie Es Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OMIE (Iberian power market), probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OMIE (Iberian power market)
provider_slug: omie-es
slug: omie-es-domain-security
source_filename: omie-es-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: omie.es\n  https: false\ndomains:\n- domain: omie.es\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/omie-es/security/omie-es-domain-security.yml
summary_line: DMARC
tags:
- Company
- Energy
- Electricity
- Market
- Spain
- Portugal
---
