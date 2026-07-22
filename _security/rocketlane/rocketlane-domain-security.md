---
api_specs:
- filename: rocketlane-openapi-original.json
  format: json
  label: Rocketlane API
  slug: rocketlane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketlane/refs/heads/main/openapi/rocketlane-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rocketlane.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: rocketlane.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rocketlane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rocketlane, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rocketlane
provider_slug: rocketlane
slug: rocketlane-domain-security
source_filename: rocketlane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rocketlane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rocketlane.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rocketlane/refs/heads/main/security/rocketlane-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Professional Services Automation
- Project Management
- Customer Onboarding
- Resource Management
- Time Tracking
- PSA
- SaaS
---
