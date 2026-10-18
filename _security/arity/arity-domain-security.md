---
api_specs:
- filename: arity-activation-api-openapi.yml
  format: yaml
  label: Arity Activation API
  slug: arity-activation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arity/refs/heads/main/openapi/arity-activation-api-openapi.yml
- filename: arity-authentication-api-openapi.yml
  format: yaml
  label: Arity Authentication API
  slug: arity-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arity/refs/heads/main/openapi/arity-authentication-api-openapi.yml
- filename: arity-booking-api-documentation-api-openapi.yml
  format: yaml
  label: Arity Booking API Documentation API
  slug: arity-booking-api-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arity/refs/heads/main/openapi/arity-booking-api-documentation-api-openapi.yml
- filename: arity-prequalcredit-api-openapi.yml
  format: yaml
  label: Arity Pre Qual Credit API
  slug: arity-prequalcredit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arity/refs/heads/main/openapi/arity-prequalcredit-api-openapi.yml
- filename: arity-registration-api-openapi.yml
  format: yaml
  label: Arity Registration API
  slug: arity-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arity/refs/heads/main/openapi/arity-registration-api-openapi.yml
- filename: arity-scoring-api-openapi.yml
  format: yaml
  label: Arity Scoring API
  slug: arity-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arity/refs/heads/main/openapi/arity-scoring-api-openapi.yml
- filename: arity-trip-intelligence-api-openapi.yml
  format: yaml
  label: Arity Trip Intelligence API
  slug: arity-trip-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arity/refs/heads/main/openapi/arity-trip-intelligence-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: arity.com
  spf: true
hosts:
- cert_expires: Nov 29 14:44:51 2026 GMT
  host: arity.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Arity
provider_slug: arity
slug: arity-domain-security
source_filename: arity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 14:44:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: arity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arity/refs/heads/main/security/arity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Telematics
- Mobility Data
- Insurance
- Driving Behavior
- Analytics
- Location Data
---
