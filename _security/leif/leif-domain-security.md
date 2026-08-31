---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leif.org
  spf: true
hosts:
- host: www.leif.org
  https: false
kind: domain-security
layout: security
method: probed
name: Leif Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leif, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Leif
provider_slug: leif
slug: leif-domain-security
source_filename: leif-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leif.org\n  https: false\ndomains:\n- domain: leif.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leif/refs/heads/main/security/leif-domain-security.yml
summary_line: DMARC
tags:
- Company
- Education
- Education Finance
- Income Share Agreement
- Student Lending
- Fintech
- Financial-Services
- Tuition
- Payments
- Lending
- New York
---
