---
api_specs:
- filename: skipodds-openapi.yml
  format: yaml
  label: SkipOdds REST API
  slug: skipodds-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skipodds/refs/heads/main/openapi/skipodds-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: skipodds.com
  spf: true
hosts:
- cert_expires: Oct 15 08:05:21 2026 GMT
  host: skipodds.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skipodds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SkipOdds, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SkipOdds
provider_slug: skipodds
slug: skipodds-domain-security
source_filename: skipodds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skipodds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 08:05:21 2026 GMT\n  hsts: null\ndomains:\n- domain: skipodds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skipodds/refs/heads/main/security/skipodds-domain-security.yml
summary_line: TLSv1.3
tags:
- sports
- odds
- probabilities
- betting-data
- de-vig
- sports-data
- real-time
- webhooks
- sports-betting
- mcp
- agent-ready
- market-data
---
