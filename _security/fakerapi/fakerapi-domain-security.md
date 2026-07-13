---
api_specs:
- filename: fakerapi-openapi.yml
  format: yaml
  label: FakerAPI
  slug: fakerapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fakerapi/refs/heads/main/openapi/fakerapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: fakerapi.it
  spf: true
hosts:
- host: fakerapi.it
  https: false
kind: domain-security
layout: security
method: probed
name: Fakerapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FakerAPI, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: FakerAPI
provider_slug: fakerapi
slug: fakerapi-domain-security
source_filename: fakerapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fakerapi.it\n  https: false\ndomains:\n- domain: fakerapi.it\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fakerapi/refs/heads/main/security/fakerapi-domain-security.yml
summary_line: DNSSEC
tags:
- Test Data
- Fake Data
- Mocking
- Developer Tools
- Open Source
- Public APIs
---
