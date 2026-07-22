---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lucirahealth.com
  spf: true
hosts:
- host: lucirahealth.com
  https: false
kind: domain-security
layout: security
method: probed
name: Lucira Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lucira Health, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lucira Health
provider_slug: lucira-health
slug: lucira-health-domain-security
source_filename: lucira-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lucirahealth.com\n  https: false\ndomains:\n- domain: lucirahealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucira-health/refs/heads/main/security/lucira-health-domain-security.yml
summary_line: DMARC
tags:
- Company
- Diagnostics
- Health
- Medical Devices
- COVID-19
- Molecular Diagnostics
- At-Home Testing
- Life Sciences
---
