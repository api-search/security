---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gastrograph.com
  spf: true
hosts:
- host: gastrograph.com
  https: false
kind: domain-security
layout: security
method: probed
name: Analytical Flavor Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Analytical Flavor Systems, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Analytical Flavor Systems
provider_slug: analytical-flavor-systems
slug: analytical-flavor-systems-domain-security
source_filename: analytical-flavor-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gastrograph.com\n  https: false\ndomains:\n- domain: gastrograph.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/analytical-flavor-systems/refs/heads/main/security/analytical-flavor-systems-domain-security.yml
summary_line: DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Food and Beverage
- Sensory Analytics
- Consumer Insights
- Flavor
---
