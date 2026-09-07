---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: acadepowder.com
  spf: true
hosts:
- host: www.acadepowder.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Acadepowder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acade Powder, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Acade Powder
provider_slug: acadepowder
slug: acadepowder-domain-security
source_filename: acadepowder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acadepowder.com\n  https: false\ndomains:\n- domain: acadepowder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acadepowder/refs/heads/main/security/acadepowder-domain-security.yml
summary_line: DMARC
tags:
- Company
- Materials
- Advanced Materials
- Metal Powder
- Additive Manufacturing
- 3D Printing
- Powder Metallurgy
- Manufacturing
- Aerospace
- China
---
