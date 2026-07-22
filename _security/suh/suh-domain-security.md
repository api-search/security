---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: suh.cn
  spf: true
hosts:
- host: suh.cn
  https: false
kind: domain-security
layout: security
method: probed
name: Suh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SinoUnited Health, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SinoUnited Health
provider_slug: suh
slug: suh-domain-security
source_filename: suh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: suh.cn\n  https: false\ndomains:\n- domain: suh.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suh/refs/heads/main/security/suh-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Healthcare
- Medical
- Dental
- Clinics
- Private Healthcare
- China
- Shanghai
---
