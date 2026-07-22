---
api_specs:
- filename: spotnana-auth-openapi-original.json
  format: json
  label: Spotnana Authentication API
  slug: spotnana-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-auth-openapi-original.json
- filename: spotnana-users-openapi-original.json
  format: json
  label: Spotnana Users API
  slug: spotnana-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-users-openapi-original.json
- filename: spotnana-company-openapi-original.json
  format: json
  label: Spotnana Company API
  slug: spotnana-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-company-openapi-original.json
- filename: spotnana-policy-openapi-original.json
  format: json
  label: Spotnana Policy API
  slug: spotnana-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-policy-openapi-original.json
- filename: spotnana-trip-openapi-original.json
  format: json
  label: Spotnana Trip API
  slug: spotnana-trip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-trip-openapi-original.json
- filename: spotnana-air-openapi-original.json
  format: json
  label: Spotnana Air API
  slug: spotnana-air-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-air-openapi-original.json
- filename: spotnana-hotel-openapi-original.json
  format: json
  label: Spotnana Hotel API
  slug: spotnana-hotel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-hotel-openapi-original.json
- filename: spotnana-event-openapi-original.json
  format: json
  label: Spotnana Event API
  slug: spotnana-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-event-openapi-original.json
- filename: spotnana-template-openapi-original.json
  format: json
  label: Spotnana Event Template API
  slug: spotnana-event-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-template-openapi-original.json
- filename: spotnana-payments-openapi-original.json
  format: json
  label: Spotnana Payments API
  slug: spotnana-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-payments-openapi-original.json
- filename: spotnana-document-openapi-original.json
  format: json
  label: Spotnana Document API
  slug: spotnana-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-document-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: spotnana.com
  spf: true
hosts:
- cert_expires: Oct 15 05:37:48 2026 GMT
  host: spotnana.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: api-ext-sboxmeta.partners.spotnana.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spotnana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spotnana, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Spotnana
provider_slug: spotnana
slug: spotnana-domain-security
source_filename: spotnana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spotnana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 05:37:48 2026 GMT\n  hsts: null\n- host: api-ext-sboxmeta.partners.spotnana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: spotnana.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/security/spotnana-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Travel
- Corporate Travel
- Travel Management
- Booking
- Air
- Hotel
- Payments
- Travel as a Service
---
