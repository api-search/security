---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sqzbiotech.com
  spf: true
hosts:
- host: sqzbiotech.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sqz Biotech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SQZ Biotech, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SQZ Biotech
provider_slug: sqz-biotech
slug: sqz-biotech-domain-security
source_filename: sqz-biotech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sqzbiotech.com\n  https: false\ndomains:\n- domain: sqzbiotech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sqz-biotech/refs/heads/main/security/sqz-biotech-domain-security.yml
summary_line: DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Cell Therapy
- Immunotherapy
- Healthcare
---
