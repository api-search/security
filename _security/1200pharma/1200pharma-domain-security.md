---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 1200pharma.com
  spf: true
hosts:
- host: 1200pharma.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 1200Pharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1200 Pharma, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 1200 Pharma
provider_slug: 1200pharma
slug: 1200pharma-domain-security
source_filename: 1200pharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1200pharma.com\n  https: false\ndomains:\n- domain: 1200pharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1200pharma/refs/heads/main/security/1200pharma-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Medicinal Chemistry
- Oncology
- Small Molecule
- Life Sciences
- Healthcare
- United States
---
