---
api_specs:
- filename: openapi
  format: yaml
  label: Octane REST API
  slug: octane-rest-api
  spec_type: OpenAPI
  url: https://docs.getoctane.io/openapi
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getoctane.io
  spf: true
hosts:
- cert_expires: Oct  8 13:02:21 2026 GMT
  host: www.getoctane.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: docs.getoctane.io
  https: false
- host: api.getoctane.io
  https: false
kind: domain-security
layout: security
method: probed
name: Octane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Octane, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Octane
provider_slug: octane
slug: octane-domain-security
source_filename: octane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getoctane.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 13:02:21 2026 GMT\n  hsts: false\n- host: docs.getoctane.io\n  https: false\n- host: api.getoctane.io\n  https: false\ndomains:\n- domain: getoctane.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/security/octane-domain-security.yml
summary_line: TLSv1.3
tags:
- Usage-Based Billing
- Metered Billing
- Pricing Plans
- SaaS Monetization
- FinTech
- Payments
- Usage Tracking
- Meters
- Entitlements
---
