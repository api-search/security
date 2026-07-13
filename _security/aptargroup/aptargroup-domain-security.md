---
api_specs:
- filename: aptargroup-openapi.yaml
  format: yaml
  label: AptarGroup API
  slug: aptargroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptargroup/refs/heads/main/openapi/aptargroup-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aptargroup.com
  spf: true
hosts:
- host: www.aptargroup.com
  https: false
- host: api.aptargroup.com
  https: false
kind: domain-security
layout: security
method: probed
name: Aptargroup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AptarGroup, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AptarGroup
provider_slug: aptargroup
slug: aptargroup-domain-security
source_filename: aptargroup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aptargroup.com\n  https: false\n- host: api.aptargroup.com\n  https: false\ndomains:\n- domain: aptargroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aptargroup/refs/heads/main/security/aptargroup-domain-security.yml
summary_line: DMARC
tags:
- Packaging
- Dispensing
- Manufacturing
- Sustainability
- Consumer Goods
- Fortune 1000
---
