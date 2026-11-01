---
api_specs:
- filename: evrotrust-all-signing-api-openapi.yml
  format: yaml
  label: Evrotrust All Signing API
  slug: evrotrust-all-signing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-all-signing-api-openapi.yml
- filename: evrotrust-e-authentication-api-openapi.yml
  format: yaml
  label: Evrotrust E Authentication API
  slug: evrotrust-e-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-e-authentication-api-openapi.yml
- filename: evrotrust-e-delivery-api-openapi.yml
  format: yaml
  label: Evrotrust E Delivery API
  slug: evrotrust-e-delivery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-e-delivery-api-openapi.yml
- filename: evrotrust-e-signatures-api-openapi.yml
  format: yaml
  label: Evrotrust E Signatures API
  slug: evrotrust-e-signatures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-e-signatures-api-openapi.yml
- filename: evrotrust-evrotrust-eid-registered-users-api-openapi.yml
  format: yaml
  label: Evrotrust Evrotrust eID (Registered Users) API
  slug: evrotrust-evrotrust-eid-registered-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-evrotrust-eid-registered-users-api-openapi.yml
- filename: evrotrust-ident-lite-advanced-basic-api-openapi.yml
  format: yaml
  label: Evrotrust Ident Lite (Advanced, Basic) API
  slug: evrotrust-ident-lite-advanced-basic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-ident-lite-advanced-basic-api-openapi.yml
- filename: evrotrust-one-time-signatures-documents-api-openapi.yml
  format: yaml
  label: Evrotrust One-time Signatures (Documents) API
  slug: evrotrust-one-time-signatures-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-one-time-signatures-documents-api-openapi.yml
- filename: evrotrust-one-time-signatures-hash-api-openapi.yml
  format: yaml
  label: Evrotrust One-time Signatures (Hash) API
  slug: evrotrust-one-time-signatures-hash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-one-time-signatures-hash-api-openapi.yml
- filename: evrotrust-signing-via-app-sdk-documents-api-openapi.yml
  format: yaml
  label: Evrotrust Signing via App/SDK (Documents) API
  slug: evrotrust-signing-via-app-sdk-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-signing-via-app-sdk-documents-api-openapi.yml
- filename: evrotrust-signing-via-app-sdk-hash-api-openapi.yml
  format: yaml
  label: Evrotrust Signing via App/SDK (Hash) API
  slug: evrotrust-signing-via-app-sdk-hash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-signing-via-app-sdk-hash-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: evrotrust.com
  spf: true
hosts:
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: evrotrust.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Evrotrust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evrotrust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Evrotrust
provider_slug: evrotrust
slug: evrotrust-domain-security
source_filename: evrotrust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evrotrust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: evrotrust.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/evrotrust/security/evrotrust-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Trust Services
- Electronic Signatures
- Digital Identity
- eIDAS
- KYC
- Identity Verification
- Timestamping
- Compliance
---
