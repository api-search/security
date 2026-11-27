---
api_specs:
- filename: bikeep-openapi-generated.yml
  format: yaml
  label: Bikeep API
  slug: bikeep-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bikeep/openapi/_ae-authored/bikeep-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bikeep.com
  spf: true
hosts:
- cert_expires: Dec 27 16:52:31 2026 GMT
  host: bikeep.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bikeep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bikeep, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bikeep
provider_slug: bikeep
slug: bikeep-domain-security
source_filename: bikeep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bikeep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 16:52:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bikeep.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/bikeep/security/bikeep-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Smart Parking
- Mobility
- IoT
- Sustainability
- Urban Infrastructure
---
