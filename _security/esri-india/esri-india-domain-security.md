---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: esriindia.com
  spf: true
hosts:
- host: www.esriindia.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Esri India Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Esri India, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Esri India
provider_slug: esri-india
slug: esri-india-domain-security
source_filename: esri-india-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.esriindia.com\n  https: false\ndomains:\n- domain: esriindia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/esri-india/security/esri-india-domain-security.yml
summary_line: DMARC
tags:
- GIS
- Mapping
- SpatialAnalytics
- EnterpriseSoftware
- India
---
