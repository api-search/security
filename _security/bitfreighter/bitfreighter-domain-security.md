---
api_specs:
- filename: bitfreighter-edi-events-api-openapi.yml
  format: yaml
  label: Bitfreighter EDI Events API
  slug: bitfreighter-edi-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitfreighter/openapi/bitfreighter-edi-events-api-openapi.yml
- filename: bitfreighter-internal-api-openapi.yml
  format: yaml
  label: Bitfreighter Internal API
  slug: bitfreighter-internal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitfreighter/openapi/bitfreighter-internal-api-openapi.yml
- filename: bitfreighter-pricing-api-openapi.yml
  format: yaml
  label: Bitfreighter Pricing API
  slug: bitfreighter-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitfreighter/openapi/bitfreighter-pricing-api-openapi.yml
- filename: bitfreighter-real-time-rating-api-openapi.yml
  format: yaml
  label: Bitfreighter Real Time Rating API
  slug: bitfreighter-real-time-rating-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitfreighter/openapi/bitfreighter-real-time-rating-api-openapi.yml
- filename: bitfreighter-sending-edi-events-api-openapi.yml
  format: yaml
  label: Bitfreighter Sending EDI Events API
  slug: bitfreighter-sending-edi-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitfreighter/openapi/bitfreighter-sending-edi-events-api-openapi.yml
- filename: bitfreighter-spot-api-openapi.yml
  format: yaml
  label: Bitfreighter Spot API
  slug: bitfreighter-spot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitfreighter/openapi/bitfreighter-spot-api-openapi.yml
- filename: bitfreighter-webhooks-api-openapi.yml
  format: yaml
  label: Bitfreighter Webhooks API
  slug: bitfreighter-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitfreighter/openapi/bitfreighter-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bitfreighter.com
  spf: true
hosts:
- cert_expires: Feb  7 17:24:47 2027 GMT
  host: bitfreighter.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bitfreighter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitfreighter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bitfreighter
provider_slug: bitfreighter
slug: bitfreighter-domain-security
source_filename: bitfreighter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitfreighter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 17:24:47 2027 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: bitfreighter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bitfreighter/security/bitfreighter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Freight
- EDI
- Logistics
---
