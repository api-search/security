---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: be.bio
  spf: true
hosts:
- host: be.bio
  https: false
kind: domain-security
layout: security
method: probed
name: Be Biopharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Be Biopharma, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Be Biopharma
provider_slug: be-biopharma
slug: be-biopharma-domain-security
source_filename: be-biopharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: be.bio\n  https: false\ndomains:\n- domain: be.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/be-biopharma/refs/heads/main/security/be-biopharma-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Biotechnology
- Life Sciences
- Cell Therapy
- Gene Therapy
- Pharmaceuticals
- Healthcare
- Clinical Trials
- Rare Disease
---
