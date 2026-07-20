---
api_specs:
- filename: aqueduct-openapi.json
  format: json
  label: Aqueduct API
  slug: aqueduct-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: tryaqueduct.com
  spf: true
hosts:
- host: www.tryaqueduct.com
  https: false
- host: api.tryaqueduct.com
  https: false
kind: domain-security
layout: security
method: probed
name: Aqueduct Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aqueduct, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Aqueduct
provider_slug: aqueduct
slug: aqueduct-domain-security
source_filename: aqueduct-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tryaqueduct.com\n  https: false\n- host: api.tryaqueduct.com\n  https: false\ndomains:\n- domain: tryaqueduct.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/security/aqueduct-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Fintech
- Billing
- Invoicing
- Metering
- Usage-Based
- Subscriptions
- Payments
- API
---
