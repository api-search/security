---
api_specs:
- filename: storable-openapi.yml
  format: yaml
  label: Storable Tenants API
  slug: storable-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Units & Rate Management API
  slug: storable-units-rate-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Ledgers & Payments API
  slug: storable-ledgers-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Leads & Reservations API
  slug: storable-leads-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Move Ins & Move Outs API
  slug: storable-move-ins-move-outs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Gate Access API
  slug: storable-gate-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Insurance API
  slug: storable-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Tasks API
  slug: storable-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Documents & eSign API
  slug: storable-documents-esign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Delinquency & Auctions API
  slug: storable-delinquency-auctions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
- filename: storable-openapi.yml
  format: yaml
  label: Storable Reporting API
  slug: storable-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/openapi/storable-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: storable.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: storedgefms.com
  spf: true
hosts:
- cert_expires: Sep 19 18:40:48 2026 GMT
  host: www.storable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 23:08:04 2026 GMT
  host: api.storedgefms.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Storable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Storable, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Storable
provider_slug: storable
slug: storable-domain-security
source_filename: storable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.storable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 18:40:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.storedgefms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:08:04 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: storable.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: storedgefms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storable/refs/heads/main/security/storable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Self Storage
- Property Management
- Facility Management
- Tenants
- Reservations
- Payments
- SiteLink
- storEDGE
- SpareFoot
---
