---
api_specs:
- filename: signsealship-closing-passports-api-openapi.yml
  format: yaml
  label: SignSealShip Partner API Closing Passports API
  slug: signsealship-closing-passports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signsealship/refs/heads/main/openapi/signsealship-closing-passports-api-openapi.yml
- filename: signsealship-closing-rooms-api-openapi.yml
  format: yaml
  label: SignSealShip Partner API Closing Rooms API
  slug: signsealship-closing-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signsealship/refs/heads/main/openapi/signsealship-closing-rooms-api-openapi.yml
- filename: signsealship-launchpad-analytics-api-openapi.yml
  format: yaml
  label: SignSealShip Partner API Launchpad & Analytics API
  slug: signsealship-launchpad-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signsealship/refs/heads/main/openapi/signsealship-launchpad-analytics-api-openapi.yml
- filename: signsealship-onboarding-api-openapi.yml
  format: yaml
  label: SignSealShip Partner API Onboarding API
  slug: signsealship-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signsealship/refs/heads/main/openapi/signsealship-onboarding-api-openapi.yml
- filename: signsealship-orders-api-openapi.yml
  format: yaml
  label: SignSealShip Partner API Orders API
  slug: signsealship-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signsealship/refs/heads/main/openapi/signsealship-orders-api-openapi.yml
- filename: signsealship-proof-passport-api-openapi.yml
  format: yaml
  label: SignSealShip Partner API Proof Passport API
  slug: signsealship-proof-passport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signsealship/refs/heads/main/openapi/signsealship-proof-passport-api-openapi.yml
- filename: signsealship-sandbox-api-openapi.yml
  format: yaml
  label: SignSealShip Partner API Sandbox API
  slug: signsealship-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signsealship/refs/heads/main/openapi/signsealship-sandbox-api-openapi.yml
- filename: signsealship-webhooks-api-openapi.yml
  format: yaml
  label: SignSealShip Partner API Webhooks API
  slug: signsealship-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signsealship/refs/heads/main/openapi/signsealship-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: signsealship.com
  spf: true
hosts:
- cert_expires: Oct 11 14:19:16 2026 GMT
  host: docs.signsealship.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 04:14:24 2026 GMT
  host: signsealship.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Signsealship Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SignSealShip Partner API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SignSealShip Partner API
provider_slug: signsealship
slug: signsealship-domain-security
source_filename: signsealship-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.signsealship.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 14:19:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: signsealship.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 04:14:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: signsealship.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signsealship/refs/heads/main/security/signsealship-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Notarization
- Remote Online Notarization
- Electronic Signature
- Document Verification
- Legal Tech
- Real Estate
- Title and Escrow
- Shipping
- A2A
---
