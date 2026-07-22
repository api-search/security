---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: landstar-system.com
  spf: false
hosts:
- host: www.landstar-system.com
  https: false
kind: domain-security
layout: security
method: probed
name: Landstar System Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Landstar System, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Landstar System
provider_slug: landstar-system
slug: landstar-system-domain-security
source_filename: landstar-system-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.landstar-system.com\n  https: false\ndomains:\n- domain: landstar-system.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landstar-system/refs/heads/main/security/landstar-system-domain-security.yml
summary_line: DMARC
tags:
- Transportation
- Trucking
- Logistics
- Supply Chain
- Fortune 1000
---
