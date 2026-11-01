---
api_specs:
- filename: satvu-openapi-generated.yml
  format: yaml
  label: SatVu API
  slug: satvu-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satvu/openapi/_ae-authored/satvu-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: satellitevu.com
  spf: true
hosts:
- cert_expires: Nov 26 13:26:09 2026 GMT
  host: www.satellitevu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Satvu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SatVu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SatVu
provider_slug: satvu
slug: satvu-domain-security
source_filename: satvu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.satellitevu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 13:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: satellitevu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/satvu/security/satvu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Thermal imagery
- Satellite data
- National security
- Economic monitoring
- Climate resilience
---
