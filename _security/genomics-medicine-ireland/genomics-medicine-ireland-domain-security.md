---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: genomicsmed.ie
  spf: true
hosts:
- host: genomicsmed.ie
  https: false
kind: domain-security
layout: security
method: probed
name: Genomics Medicine Ireland Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genomics Medicine Ireland, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Genomics Medicine Ireland
provider_slug: genomics-medicine-ireland
slug: genomics-medicine-ireland-domain-security
source_filename: genomics-medicine-ireland-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genomicsmed.ie\n  https: false\ndomains:\n- domain: genomicsmed.ie\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genomics-medicine-ireland/refs/heads/main/security/genomics-medicine-ireland-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Life Sciences
- Genomics
- Precision Medicine
- Healthcare
- Biotechnology
- Genetic Research
- Ireland
---
