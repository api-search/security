---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bioregenmed.com
  spf: true
hosts:
- host: www.bioregenmed.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bioregenmed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bioregenmed, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bioregenmed
provider_slug: bioregenmed
slug: bioregenmed-domain-security
source_filename: bioregenmed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bioregenmed.com\n  https: false\ndomains:\n- domain: bioregenmed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bioregenmed/refs/heads/main/security/bioregenmed-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Biomedical
- Materials
- TissueRepair
- China
- Medical Devices
---
