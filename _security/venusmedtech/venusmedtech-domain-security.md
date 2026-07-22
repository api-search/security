---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: venusmedtech.com
  spf: true
hosts:
- host: venusmedtech.com
  https: false
kind: domain-security
layout: security
method: probed
name: Venusmedtech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for venusmedtech, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: venusmedtech
provider_slug: venusmedtech
slug: venusmedtech-domain-security
source_filename: venusmedtech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: venusmedtech.com\n  https: false\ndomains:\n- domain: venusmedtech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/venusmedtech/refs/heads/main/security/venusmedtech-domain-security.yml
summary_line: DMARC
tags:
- Company
- Medical Devices
- MedTech
- Structural Heart
- Cardiovascular
- Heart Valves
- Healthcare
- China
---
