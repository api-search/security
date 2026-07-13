---
api_specs:
- filename: jservice-openapi.yml
  format: yaml
  label: jService Trivia API
  slug: jservice-trivia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jservice/refs/heads/main/openapi/jservice-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: jservice.io
  spf: true
hosts:
- host: jservice.io
  https: false
kind: domain-security
layout: security
method: probed
name: Jservice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for jService, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: jService
provider_slug: jservice
slug: jservice-domain-security
source_filename: jservice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jservice.io\n  https: false\ndomains:\n- domain: jservice.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jservice/refs/heads/main/security/jservice-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Games And Comics
- Trivia
- Jeopardy
- Open Source
- Ruby
- Rails
- Public APIs
---
