---
api_specs:
- filename: romit-openapi.yml
  format: yaml
  label: Romit API
  slug: romit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/romit/refs/heads/main/openapi/romit-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: romit.io
  spf: false
hosts:
- host: api.romit.io
  https: false
- host: api.sandbox.romit.io
  https: false
kind: domain-security
layout: security
method: probed
name: Romit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Romit, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Romit
provider_slug: romit
slug: romit-domain-security
source_filename: romit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  Romit (romit.io) is defunct; the API hosts no longer serve HTTPS. Absence of\n  records below is valid probed data for the dead domain.\nhosts:\n- host: api.romit.io\n  https: false\n- host: api.sandbox.romit.io\n  https: false\ndomains:\n- domain: romit.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/romit/refs/heads/main/security/romit-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Payments
- Fintech
- Digital Wallet
- Payment Gateway
- Merchant Services
- Chargebacks
- Fraud Prevention
- Invoicing
- Subscriptions
---
