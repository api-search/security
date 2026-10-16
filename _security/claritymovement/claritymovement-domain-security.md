---
api_specs:
- filename: claritymovement-openapi-generated.yml
  format: yaml
  label: Claritymovement API
  slug: claritymovement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claritymovement/refs/heads/main/openapi/_ae-authored/claritymovement-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clarity.io
  spf: true
hosts:
- cert_expires: Nov 24 19:48:01 2026 GMT
  host: www.clarity.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Claritymovement Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Claritymovement, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Claritymovement
provider_slug: claritymovement
slug: claritymovement-domain-security
source_filename: claritymovement-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clarity.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 19:48:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clarity.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claritymovement/refs/heads/main/security/claritymovement-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AirQuality
- IoT
- Sensors
- DataAnalytics
---
