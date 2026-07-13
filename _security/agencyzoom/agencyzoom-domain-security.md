---
api_specs:
- filename: agencyzoom.yaml
  format: yaml
  label: AgencyZoom API
  slug: api
  spec_type: OpenAPI
  url: https://app.agencyzoom.com/openapi/agencyzoom.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agencyzoom.com
  spf: true
hosts:
- cert_expires: Aug 18 21:56:07 2026 GMT
  host: agencyzoom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: app.agencyzoom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: api.agencyzoom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agencyzoom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgencyZoom, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AgencyZoom
provider_slug: agencyzoom
slug: agencyzoom-domain-security
source_filename: agencyzoom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agencyzoom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 21:56:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.agencyzoom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.agencyzoom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agencyzoom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/security/agencyzoom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- InsurTech
- CRM
- Sales Automation
- Agency Management
- Customer Retention
---
