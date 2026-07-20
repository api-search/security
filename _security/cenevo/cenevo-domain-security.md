---
api_specs:
- filename: cenevo-labguru-v1-openapi.yml
  format: yaml
  label: Labguru API v1
  slug: labguru-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cenevo/refs/heads/main/openapi/cenevo-labguru-v1-openapi.yml
- filename: cenevo-labguru-v2-openapi.yml
  format: yaml
  label: Labguru API v2
  slug: labguru-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cenevo/refs/heads/main/openapi/cenevo-labguru-v2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: labguru.com
  spf: true
hosts:
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: my.labguru.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cenevo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cenevo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cenevo
provider_slug: cenevo
slug: cenevo-domain-security
source_filename: cenevo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: my.labguru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: labguru.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cenevo/refs/heads/main/security/cenevo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Lab Automation
- Laboratory Informatics
- Electronic Lab Notebook
- LIMS
- Sample Management
- Life Sciences
- Biotechnology
- Scientific Research
- AI Agents
- Data Management
---
