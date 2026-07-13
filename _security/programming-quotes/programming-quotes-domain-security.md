---
api_specs:
- filename: programming-quotes-openapi.yml
  format: yaml
  label: Programming Quotes
  slug: programming-quotes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/programming-quotes/refs/heads/main/openapi/programming-quotes-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: azurewebsites.net
  spf: false
hosts:
- host: programming-quotes-api.azurewebsites.net
  https: false
kind: domain-security
layout: security
method: probed
name: Programming Quotes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Programming Quotes, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Programming Quotes
provider_slug: programming-quotes
slug: programming-quotes-domain-security
source_filename: programming-quotes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: programming-quotes-api.azurewebsites.net\n  https: false\ndomains:\n- domain: azurewebsites.net\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/programming-quotes/refs/heads/main/security/programming-quotes-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Personality
- Public APIs
- Open Source
- Quotes
- Programming
- Developer Tools
---
