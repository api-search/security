---
api_specs:
- filename: gbg-as-api-openapi.yml
  format: yaml
  label: GBG As API
  slug: gbg-as-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-as-api-openapi.yml
- filename: gbg-authentication-api-openapi.yml
  format: yaml
  label: GBG Authentication API
  slug: gbg-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-authentication-api-openapi.yml
- filename: gbg-customer-apis-api-openapi.yml
  format: yaml
  label: GBG Customer APIs API
  slug: gbg-customer-apis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-customer-apis-api-openapi.yml
- filename: gbg-device-api-openapi.yml
  format: yaml
  label: GBG Device API
  slug: gbg-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-device-api-openapi.yml
- filename: gbg-end-user-apis-api-openapi.yml
  format: yaml
  label: GBG End User APIs API
  slug: gbg-end-user-apis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-end-user-apis-api-openapi.yml
- filename: gbg-health-api-openapi.yml
  format: yaml
  label: GBG Health API
  slug: gbg-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-health-api-openapi.yml
- filename: gbg-interaction-api-openapi.yml
  format: yaml
  label: GBG Interaction API
  slug: gbg-interaction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-interaction-api-openapi.yml
- filename: gbg-interaction-service-api-openapi.yml
  format: yaml
  label: GBG Interaction Service API
  slug: gbg-interaction-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-interaction-service-api-openapi.yml
- filename: gbg-journey-api-openapi.yml
  format: yaml
  label: GBG Journey API
  slug: gbg-journey-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-journey-api-openapi.yml
- filename: gbg-journey-execution-api-openapi.yml
  format: yaml
  label: GBG Journey execution API
  slug: gbg-journey-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-journey-execution-api-openapi.yml
- filename: gbg-sandbox-api-openapi.yml
  format: yaml
  label: GBG Sandbox API
  slug: gbg-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbg/openapi/gbg-sandbox-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gbgplc.com
  spf: true
hosts:
- cert_expires: Jan 14 09:56:27 2027 GMT
  host: gbgplc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gbg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GBG, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GBG
provider_slug: gbg
slug: gbg-domain-security
source_filename: gbg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gbgplc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 09:56:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gbgplc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gbg/security/gbg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Identity Verification
- Fraud Prevention
- KYC
- Location Intelligence
- Compliance
- Digital Identity
---
