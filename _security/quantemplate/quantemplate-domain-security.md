---
api_specs:
- filename: quantemplate-fabric-openapi.yml
  format: yaml
  label: Quantemplate FabricAPI
  slug: quantemplate-fabricapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quantemplate/refs/heads/main/openapi/quantemplate-fabric-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quantemplate.com
  spf: true
hosts:
- cert_expires: Sep 11 20:25:28 2026 GMT
  host: quantemplate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quantemplate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QuanTemplate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: QuanTemplate
provider_slug: quantemplate
slug: quantemplate-domain-security
source_filename: quantemplate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quantemplate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 20:25:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: quantemplate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantemplate/refs/heads/main/security/quantemplate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Insurtech
- Data Integration
- Data Management
- Bordereaux
- Data Validation
- Pipelines
- Analytics
- No-Code
- API
---
