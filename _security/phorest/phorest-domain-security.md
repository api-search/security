---
api_specs:
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Clients API
  slug: phorest-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Appointments & Bookings API
  slug: phorest-appointments-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Staff API
  slug: phorest-staff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Services API
  slug: phorest-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Products & Purchases API
  slug: phorest-products-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Vouchers & Loyalty API
  slug: phorest-vouchers-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Branches API
  slug: phorest-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Reporting & Reviews API
  slug: phorest-reporting-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "amazontrust.com"
  - 0 issue "amazonaws.com"
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: phorest.com
  spf: true
hosts:
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: www.phorest.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 26 08:43:26 2026 GMT
  host: developer.phorest.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: api-gateway-eu.phorest.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Phorest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phorest, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Phorest
provider_slug: phorest
slug: phorest-domain-security
source_filename: phorest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.phorest.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.phorest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 08:43:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-gateway-eu.phorest.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: phorest.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/security/phorest-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Salon Software
- Spa Software
- Scheduling
- Point of Sale
- Business Management
- Vertical SaaS
---
