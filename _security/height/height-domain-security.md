---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Height REST API
  slug: height-api
  spec_type: OpenAPI
  url: https://height-api.xyz/openapi/
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: height.app
  spf: true
hosts:
- host: height.app
  https: false
- host: api.height.app
  https: false
kind: domain-security
layout: security
method: probed
name: Height Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Height, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Height
provider_slug: height
slug: height-domain-security
source_filename: height-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: height.app\n  https: false\n- host: api.height.app\n  https: false\ndomains:\n- domain: height.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/security/height-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Project Management
- Task Management
- Collaboration
- Productivity
- Workflow Automation
- AI
---
