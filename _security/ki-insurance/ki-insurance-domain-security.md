---
api_specs:
- filename: ki-insurance-broker-platform-openapi.yml
  format: yaml
  label: Ki Broker Trading Platform API
  slug: broker-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-broker-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ki-insurance.com
  spf: true
hosts:
- cert_expires: Oct 21 23:19:28 2026 GMT
  host: ki-insurance.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 06:59:10 2026 GMT
  host: app.ki-insurance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ki Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ki Insurance, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ki Insurance
provider_slug: ki-insurance
slug: ki-insurance-domain-security
source_filename: ki-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ki-insurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:19:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.ki-insurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 06:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ki-insurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/security/ki-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- Lloyd's of London
- Specialty Insurance
- Property and Casualty
- Underwriting
- Insurtech
- Broker
- Algorithmic Underwriting
- Reinsurance
---
