---
api_specs:
- filename: digital-turbine-openapi-generated.yml
  format: yaml
  label: Digital Turbine (Fyber) API
  slug: digital-turbine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/digital-turbine/openapi/_ae-authored/digital-turbine-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: digitalturbine.com
  spf: true
hosts:
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: www.digitalturbine.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Digital Turbine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digital Turbine (Fyber), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Digital Turbine (Fyber)
provider_slug: digital-turbine
slug: digital-turbine-domain-security
source_filename: digital-turbine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.digitalturbine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: digitalturbine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/digital-turbine/security/digital-turbine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mobile
- Advertising
- Monetization
- SDK
---
