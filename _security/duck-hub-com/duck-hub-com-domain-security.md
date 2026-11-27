---
api_specs:
- filename: duck-hub-com-integrationspublic-api-openapi.yml
  format: yaml
  label: Duckhub Integrations Public API
  slug: duck-hub-com-integrationspublic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duck-hub-com/openapi/duck-hub-com-integrationspublic-api-openapi.yml
- filename: duck-hub-com-open-api-api-openapi.yml
  format: yaml
  label: Duckhub Open API
  slug: duck-hub-com-open-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duck-hub-com/openapi/duck-hub-com-open-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: duck-hub.com
  spf: true
hosts:
- cert_expires: Dec 18 08:38:35 2026 GMT
  host: duck-hub.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Duckhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Duckhub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Duckhub
provider_slug: duck-hub-com
slug: duck-hub-com-domain-security
source_filename: duck-hub-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: duck-hub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 08:38:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: duck-hub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/duck-hub-com/security/duck-hub-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- QR
- Restaurant
- Software-as-a-Service
- Menus
- Company
---
