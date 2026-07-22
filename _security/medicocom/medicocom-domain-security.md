---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: medico.com
  spf: true
hosts:
- host: medico.com
  https: false
kind: domain-security
layout: security
method: probed
name: Medicocom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medico.com, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Medico.com
provider_slug: medicocom
slug: medicocom-domain-security
source_filename: medicocom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medico.com\n  https: false\ndomains:\n- domain: medico.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medicocom/refs/heads/main/security/medicocom-domain-security.yml
summary_line: DMARC
tags:
- Company
- Health
- Healthcare
- Consumer Health
- Q&A Community
- Acquired
- Everyday Health
---
