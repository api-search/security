---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: humedica.com
  spf: true
hosts:
- host: www.humedica.com
  https: false
kind: domain-security
layout: security
method: probed
name: Humedica Unitedhealth Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Humedica (UnitedHealth Group), probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Humedica (UnitedHealth Group)
provider_slug: humedica-unitedhealth-group
slug: humedica-unitedhealth-group-domain-security
source_filename: humedica-unitedhealth-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.humedica.com\n  https: false\ndomains:\n- domain: humedica.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humedica-unitedhealth-group/refs/heads/main/security/humedica-unitedhealth-group-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Ai Apps
- Healthcare
- Health Analytics
- Clinical Data
- Optum
- UnitedHealth Group
---
