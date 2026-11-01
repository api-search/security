---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tripod-glp.com
  spf: true
hosts:
- host: tripod-glp.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tripod Glp Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tripod-glp, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: tripod-glp
provider_slug: tripod-glp-com
slug: tripod-glp-com-domain-security
source_filename: tripod-glp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tripod-glp.com\n  https: false\ndomains:\n- domain: tripod-glp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/tripod-glp-com/security/tripod-glp-com-domain-security.yml
summary_line: DMARC
tags:
- Company
- Logistics
- Cloud
- API
- Supply-Chain
---
