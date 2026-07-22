---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: independencehealthgroup.com
  spf: true
hosts:
- host: www.independencehealthgroup.com
  https: false
kind: domain-security
layout: security
method: probed
name: Independence Health Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Independence Health Group, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Independence Health Group
provider_slug: independence-health-group
slug: independence-health-group-domain-security
source_filename: independence-health-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.independencehealthgroup.com\n  https: false\ndomains:\n- domain: independencehealthgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/independence-health-group/refs/heads/main/security/independence-health-group-domain-security.yml
summary_line: DMARC
tags:
- Healthcare
- Health Insurance
- Holding Company
- Insurance
- Managed Care
---
