---
api_specs:
- filename: drivings-com-discovery-api-openapi.yml
  format: yaml
  label: Drivings Discovery API
  slug: drivings-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drivings-com/openapi/drivings-com-discovery-api-openapi.yml
- filename: drivings-com-planning-api-openapi.yml
  format: yaml
  label: Drivings Planning API
  slug: drivings-com-planning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drivings-com/openapi/drivings-com-planning-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: drivings.com
  spf: false
hosts:
- cert_expires: Dec 10 12:57:15 2026 GMT
  host: drivings.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Drivings Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drivings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Drivings
provider_slug: drivings-com
slug: drivings-com-domain-security
source_filename: drivings-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drivings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 12:57:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: drivings.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/drivings-com/security/drivings-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Driving
- Education
- United Kingdom
- US
---
