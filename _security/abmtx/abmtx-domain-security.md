---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: abmtx.com
  spf: true
hosts:
- host: www.abmtx.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Abmtx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ABM Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ABM Therapeutics
provider_slug: abmtx
slug: abmtx-domain-security
source_filename: abmtx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abmtx.com\n  https: false\ndomains:\n- domain: abmtx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abmtx/refs/heads/main/security/abmtx-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Oncology
- Drug Discovery
- Clinical Trials
- Healthcare
---
