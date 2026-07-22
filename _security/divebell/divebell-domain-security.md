---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: divebell.com
  spf: true
hosts:
- host: www.divebell.com
  https: false
kind: domain-security
layout: security
method: probed
name: Divebell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Divebell, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Divebell
provider_slug: divebell
slug: divebell-domain-security
source_filename: divebell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.divebell.com\n  https: false\ndomains:\n- domain: divebell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/divebell/refs/heads/main/security/divebell-domain-security.yml
summary_line: DMARC
tags:
- Company
- Data Privacy
- Data Discovery
- Data Classification
- PII
- Compliance
- Data Subject Requests
- Risk Management
- Data Security
- Data Governance
---
