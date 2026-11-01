---
api_specs:
- filename: wiastandards-com-domains-api-openapi.yml
  format: yaml
  label: wiastandards-com Domains API
  slug: wiastandards-com-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wiastandards-com/openapi/wiastandards-com-domains-api-openapi.yml
- filename: wiastandards-com-keys-api-openapi.yml
  format: yaml
  label: wiastandards-com Keys API
  slug: wiastandards-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wiastandards-com/openapi/wiastandards-com-keys-api-openapi.yml
- filename: wiastandards-com-standards-api-openapi.yml
  format: yaml
  label: wiastandards-com Standards API
  slug: wiastandards-com-standards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wiastandards-com/openapi/wiastandards-com-standards-api-openapi.yml
- filename: wiastandards-com-usage-api-openapi.yml
  format: yaml
  label: wiastandards-com Usage API
  slug: wiastandards-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wiastandards-com/openapi/wiastandards-com-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wiastandards.com
  spf: true
hosts:
- cert_expires: Dec 16 03:27:34 2026 GMT
  host: wiastandards.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wiastandards Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for wiastandards-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: wiastandards-com
provider_slug: wiastandards-com
slug: wiastandards-com-domain-security
source_filename: wiastandards-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wiastandards.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 03:27:34 2026 GMT\n  hsts: false\ndomains:\n- domain: wiastandards.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/wiastandards-com/security/wiastandards-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Standards
- Certification
- Interoperability
- Digital-Twin
- Data-Exchange
---
