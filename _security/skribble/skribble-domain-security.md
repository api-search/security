---
api_specs:
- filename: skribble-access-api-openapi.yml
  format: yaml
  label: Skribble Access API
  slug: skribble-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-access-api-openapi.yml
- filename: skribble-additional-information-api-openapi.yml
  format: yaml
  label: Skribble Additional Information API
  slug: skribble-additional-information-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-additional-information-api-openapi.yml
- filename: skribble-billing-and-credits-api-openapi.yml
  format: yaml
  label: Skribble Billing and Credits API
  slug: skribble-billing-and-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-billing-and-credits-api-openapi.yml
- filename: skribble-document-api-openapi.yml
  format: yaml
  label: Skribble Document API
  slug: skribble-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-document-api-openapi.yml
- filename: skribble-identification-api-openapi.yml
  format: yaml
  label: Skribble Identification API
  slug: skribble-identification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-identification-api-openapi.yml
- filename: skribble-monitoring-api-openapi.yml
  format: yaml
  label: Skribble Monitoring API
  slug: skribble-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-monitoring-api-openapi.yml
- filename: skribble-report-api-openapi.yml
  format: yaml
  label: Skribble Report API
  slug: skribble-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-report-api-openapi.yml
- filename: skribble-reports-api-openapi.yml
  format: yaml
  label: Skribble Reports API
  slug: skribble-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-reports-api-openapi.yml
- filename: skribble-seal-api-openapi.yml
  format: yaml
  label: Skribble Seal API
  slug: skribble-seal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-seal-api-openapi.yml
- filename: skribble-sendto-api-openapi.yml
  format: yaml
  label: Skribble Send To API
  slug: skribble-sendto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-sendto-api-openapi.yml
- filename: skribble-signature-api-openapi.yml
  format: yaml
  label: Skribble Signature API
  slug: skribble-signature-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-signature-api-openapi.yml
- filename: skribble-signature-attachment-api-openapi.yml
  format: yaml
  label: Skribble Signature Attachment API
  slug: skribble-signature-attachment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-signature-attachment-api-openapi.yml
- filename: skribble-signature-handling-api-openapi.yml
  format: yaml
  label: Skribble Signature Handling API
  slug: skribble-signature-handling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-signature-handling-api-openapi.yml
- filename: skribble-signature-observer-api-openapi.yml
  format: yaml
  label: Skribble Signature Observer API
  slug: skribble-signature-observer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-signature-observer-api-openapi.yml
- filename: skribble-signature-signer-api-openapi.yml
  format: yaml
  label: Skribble Signature Signer API
  slug: skribble-signature-signer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-signature-signer-api-openapi.yml
- filename: skribble-user-api-openapi.yml
  format: yaml
  label: Skribble User API
  slug: skribble-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-user-api-openapi.yml
- filename: skribble-validation-api-openapi.yml
  format: yaml
  label: Skribble Validation API
  slug: skribble-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-validation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: skribble.com
  spf: true
hosts:
- cert_expires: Nov 21 04:43:53 2026 GMT
  host: skribble.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Skribble Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skribble, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Skribble
provider_slug: skribble
slug: skribble-domain-security
source_filename: skribble-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skribble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 04:43:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: skribble.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/skribble/security/skribble-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Signature
- Digital Signature
- Qualified Electronic Signature
- Signature Validation
- eIDAS
- Switzerland
---
