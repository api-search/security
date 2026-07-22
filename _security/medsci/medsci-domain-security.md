---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: medsci.cn
  spf: true
hosts:
- host: medsci.cn
  https: false
kind: domain-security
layout: security
method: probed
name: Medsci Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MedSci, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MedSci
provider_slug: medsci
slug: medsci-domain-security
source_filename: medsci-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medsci.cn\n  https: false\ndomains:\n- domain: medsci.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medsci/refs/heads/main/security/medsci-domain-security.yml
summary_line: DMARC
tags:
- Company
- Healthcare
- Medical
- Physician Platform
- Artificial Intelligence
- Real-World Evidence
- China
---
