---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thepta.com
  spf: true
hosts:
- host: thepta.com
  https: false
kind: domain-security
layout: security
method: probed
name: Pta Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PTA Networks, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PTA Networks
provider_slug: pta-networks
slug: pta-networks-domain-security
source_filename: pta-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thepta.com\n  https: false\ndomains:\n- domain: thepta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pta-networks/refs/heads/main/security/pta-networks-domain-security.yml
summary_line: DMARC
tags:
- Company
---
