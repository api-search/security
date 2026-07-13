---
api_specs:
- filename: terapi-openapi.yml
  format: yaml
  label: Terapi API
  slug: terapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terapi/refs/heads/main/openapi/terapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: terapi.dev
  spf: true
hosts:
- host: terapi.dev
  https: false
- host: api.terapi.dev
  https: false
kind: domain-security
layout: security
method: probed
name: Terapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terapi, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Terapi
provider_slug: terapi
slug: terapi-domain-security
source_filename: terapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: terapi.dev\n  https: false\n- host: api.terapi.dev\n  https: false\ndomains:\n- domain: terapi.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terapi/refs/heads/main/security/terapi-domain-security.yml
summary_line: DMARC
tags:
- Authentication
- Connectors
- Embedded iPaaS
- Integration
- Native Integrations
- Open Source
- Workflow Automation
---
