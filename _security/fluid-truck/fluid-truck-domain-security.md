---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fluidtruck.com
  spf: true
hosts:
- host: fluidtruck.com
  https: false
kind: domain-security
layout: security
method: probed
name: Fluid Truck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fluid Truck, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fluid Truck
provider_slug: fluid-truck
slug: fluid-truck-domain-security
source_filename: fluid-truck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fluidtruck.com\n  https: false\ndomains:\n- domain: fluidtruck.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fluid-truck/refs/heads/main/security/fluid-truck-domain-security.yml
summary_line: DMARC
tags:
- Company
- Transportation
- Logistics
- Vehicle Rental
- Fleet Management
- Mobility
- Marketplace
- Defunct
---
