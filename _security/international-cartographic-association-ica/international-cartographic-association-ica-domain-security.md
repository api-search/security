---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: icaci.org
  spf: true
hosts:
- host: icaci.org
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: International Cartographic Association Ica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for International Cartographic Association ICA, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: International Cartographic Association ICA
provider_slug: international-cartographic-association-ica
slug: international-cartographic-association-ica-domain-security
source_filename: international-cartographic-association-ica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: icaci.org\n  https: false\ndomains:\n- domain: icaci.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/international-cartographic-association-ica/security/international-cartographic-association-ica-domain-security.yml
summary_line: DMARC
tags:
- Cartography
- GIScience
- Geography
- Nonprofit
- International
---
