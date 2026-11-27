---
api_specs:
- filename: freightutils-com-adr-api-openapi.yml
  format: yaml
  label: FreightUtils ADR API
  slug: freightutils-com-adr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freightutils-com/openapi/freightutils-com-adr-api-openapi.yml
- filename: freightutils-com-calculators-api-openapi.yml
  format: yaml
  label: FreightUtils Calculators API
  slug: freightutils-com-calculators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freightutils-com/openapi/freightutils-com-calculators-api-openapi.yml
- filename: freightutils-com-composite-api-openapi.yml
  format: yaml
  label: FreightUtils Composite API
  slug: freightutils-com-composite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freightutils-com/openapi/freightutils-com-composite-api-openapi.yml
- filename: freightutils-com-consignment-api-openapi.yml
  format: yaml
  label: FreightUtils Consignment API
  slug: freightutils-com-consignment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freightutils-com/openapi/freightutils-com-consignment-api-openapi.yml
- filename: freightutils-com-customs-api-openapi.yml
  format: yaml
  label: FreightUtils Customs API
  slug: freightutils-com-customs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freightutils-com/openapi/freightutils-com-customs-api-openapi.yml
- filename: freightutils-com-reference-api-openapi.yml
  format: yaml
  label: FreightUtils Reference API
  slug: freightutils-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freightutils-com/openapi/freightutils-com-reference-api-openapi.yml
- filename: freightutils-com-reference-data-api-openapi.yml
  format: yaml
  label: FreightUtils Reference Data API
  slug: freightutils-com-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freightutils-com/openapi/freightutils-com-reference-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: freightutils.com
  spf: true
hosts:
- cert_expires: Dec 14 17:37:24 2026 GMT
  host: freightutils.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FreightUtils Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreightUtils, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FreightUtils
provider_slug: freightutils-com
slug: freightutils-com-domain-security
source_filename: freightutils-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freightutils.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 17:37:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: freightutils.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/freightutils-com/security/freightutils-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Freight
- Data
---
