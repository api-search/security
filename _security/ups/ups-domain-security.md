---
api_specs:
- filename: ups-address-validation-api-openapi.yml
  format: yaml
  label: UPS Address Validation API
  slug: ups-address-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-address-validation-api-openapi.yml
- filename: ups-oauth-api-openapi.yml
  format: yaml
  label: UPS OAuth API
  slug: ups-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-oauth-api-openapi.yml
- filename: ups-paperless-documents-api-openapi.yml
  format: yaml
  label: UPS Paperless Documents API
  slug: ups-paperless-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-paperless-documents-api-openapi.yml
- filename: ups-pickup-api-openapi.yml
  format: yaml
  label: UPS Pickup API
  slug: ups-pickup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-pickup-api-openapi.yml
- filename: ups-rating-api-openapi.yml
  format: yaml
  label: UPS Rating API
  slug: ups-rating-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-rating-api-openapi.yml
- filename: ups-shipping-api-openapi.yml
  format: yaml
  label: UPS Shipping API
  slug: ups-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-shipping-api-openapi.yml
- filename: ups-time-in-transit-api-openapi.yml
  format: yaml
  label: UPS Time In Transit API
  slug: ups-time-in-transit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-time-in-transit-api-openapi.yml
- filename: ups-tracking-api-openapi.yml
  format: yaml
  label: UPS Tracking API
  slug: ups-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-tracking-api-openapi.yml
description: ''
domains:
- caa:
  - 128 issue "ica.cz"
  - 128 issue "globalsign.com"
  - 128 issue "sectigo.com"
  - 128 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ups.com
  spf: true
hosts:
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: www.ups.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: developer.ups.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: onlinetools.ups.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ups Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UPS, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: UPS
provider_slug: ups
slug: ups-domain-security
source_filename: ups-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ups.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: null\n- host: developer.ups.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: null\n- host: onlinetools.ups.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ups.com\n  dnssec: true\n  caa:\n  - 128 issue \"ica.cz\"\n  - 128 issue \"globalsign.com\"\n  - 128 issue \"sectigo.com\"\n  - 128 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/security/ups-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Logistics
- Shipping
- Fortune 500
- Supply Chain
---
