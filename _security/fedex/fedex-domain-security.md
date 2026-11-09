---
api_specs:
- filename: fedex-authorization-api-openapi.yml
  format: yaml
  label: FedEx API Authorization
  slug: fedex-api-authorization
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-authorization-api-openapi.yml
- filename: fedex-rate-api-openapi.yml
  format: yaml
  label: FedEx Rates and Transit Times API
  slug: fedex-rates-and-transit-times-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-rate-api-openapi.yml
- filename: fedex-ship-api-openapi.yml
  format: yaml
  label: FedEx Ship API
  slug: fedex-ship-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-ship-api-openapi.yml
- filename: fedex-pickup-api-openapi.yml
  format: yaml
  label: FedEx Pickup Request API
  slug: fedex-pickup-request-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-pickup-api-openapi.yml
- filename: fedex-track-api-openapi.yml
  format: yaml
  label: FedEx Basic Integrated Visibility
  slug: fedex-basic-integrated-visibility
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-track-api-openapi.yml
- filename: fedex-regulatory-api-openapi.yml
  format: yaml
  label: FedEx Regulatory API
  slug: fedex-regulatory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-regulatory-api-openapi.yml
- filename: fedex-address-api-openapi.yml
  format: yaml
  label: FedEx Address API
  slug: fedex-address-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-address-api-openapi.yml
- filename: fedex-availability-api-openapi.yml
  format: yaml
  label: FedEx Availability API
  slug: fedex-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-availability-api-openapi.yml
- filename: fedex-commodity-api-openapi.yml
  format: yaml
  label: FedEx Commodity API
  slug: fedex-commodity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-commodity-api-openapi.yml
- filename: fedex-country-api-openapi.yml
  format: yaml
  label: FedEx Country API
  slug: fedex-country-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-country-api-openapi.yml
- filename: fedex-documents-api-openapi.yml
  format: yaml
  label: FedEx Documents API
  slug: fedex-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-documents-api-openapi.yml
- filename: fedex-dutytax-api-openapi.yml
  format: yaml
  label: FedEx Dutytax API
  slug: fedex-dutytax-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-dutytax-api-openapi.yml
- filename: fedex-globaltrade-api-openapi.yml
  format: yaml
  label: FedEx Globaltrade API
  slug: fedex-globaltrade-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-globaltrade-api-openapi.yml
- filename: fedex-irc-api-openapi.yml
  format: yaml
  label: FedEx Irc API
  slug: fedex-irc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-irc-api-openapi.yml
- filename: fedex-location-api-openapi.yml
  format: yaml
  label: FedEx Location API
  slug: fedex-location-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-location-api-openapi.yml
- filename: fedex-webhook-api-openapi.yml
  format: yaml
  label: FedEx Webhook API
  slug: fedex-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-webhook-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "identrust.com"
  - 0 iodef "mailto:hostmaster@fedex.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fedex.com
  spf: true
hosts:
- cert_expires: Sep  5 23:59:59 2026 GMT
  host: www.fedex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 23:59:59 2026 GMT
  host: developer.fedex.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: apis.fedex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Fedex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FedEx, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FedEx
provider_slug: fedex
slug: fedex-domain-security
source_filename: fedex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fedex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:59:59 2026 GMT\n  hsts: null\n- host: developer.fedex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: apis.fedex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fedex.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"identrust.com\"\n  - 0 iodef \"mailto:hostmaster@fedex.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fedex/security/fedex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Address Validation
- Freight
- Logistics
- Pickup
- Ratings
- Shipping
- Tracking
- Webhook
- Fortune 100
---
