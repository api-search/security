---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gxo-logistics.com
  spf: false
hosts:
- host: www.gxo-logistics.com
  https: false
kind: domain-security
layout: security
method: probed
name: Gxo Logistics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for gxo-logistics, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: gxo-logistics
provider_slug: gxo-logistics
slug: gxo-logistics-domain-security
source_filename: gxo-logistics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gxo-logistics.com\n  https: false\ndomains:\n- domain: gxo-logistics.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gxo-logistics/refs/heads/main/security/gxo-logistics-domain-security.yml
summary_line: DMARC
tags: []
---
