---
api_specs:
- filename: wellnessliving-appointments-api-openapi.yml
  format: yaml
  label: WellnessLiving Appointments API
  slug: wellnessliving-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-appointments-api-openapi.yml
- filename: wellnessliving-authentication-api-openapi.yml
  format: yaml
  label: WellnessLiving Authentication API
  slug: wellnessliving-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-authentication-api-openapi.yml
- filename: wellnessliving-booking-api-openapi.yml
  format: yaml
  label: WellnessLiving Booking API
  slug: wellnessliving-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-booking-api-openapi.yml
- filename: wellnessliving-business-api-openapi.yml
  format: yaml
  label: WellnessLiving Business API
  slug: wellnessliving-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-business-api-openapi.yml
- filename: wellnessliving-catalog-api-openapi.yml
  format: yaml
  label: WellnessLiving Catalog API
  slug: wellnessliving-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-catalog-api-openapi.yml
- filename: wellnessliving-classes-api-openapi.yml
  format: yaml
  label: WellnessLiving Classes API
  slug: wellnessliving-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-classes-api-openapi.yml
- filename: wellnessliving-clients-api-openapi.yml
  format: yaml
  label: WellnessLiving Clients API
  slug: wellnessliving-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-clients-api-openapi.yml
- filename: wellnessliving-locations-api-openapi.yml
  format: yaml
  label: WellnessLiving Locations API
  slug: wellnessliving-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-locations-api-openapi.yml
- filename: wellnessliving-payments-api-openapi.yml
  format: yaml
  label: WellnessLiving Payments API
  slug: wellnessliving-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-payments-api-openapi.yml
- filename: wellnessliving-promotions-api-openapi.yml
  format: yaml
  label: WellnessLiving Promotions API
  slug: wellnessliving-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-promotions-api-openapi.yml
- filename: wellnessliving-reports-api-openapi.yml
  format: yaml
  label: WellnessLiving Reports API
  slug: wellnessliving-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-reports-api-openapi.yml
- filename: wellnessliving-reviews-api-openapi.yml
  format: yaml
  label: WellnessLiving Reviews API
  slug: wellnessliving-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-reviews-api-openapi.yml
- filename: wellnessliving-rewards-api-openapi.yml
  format: yaml
  label: WellnessLiving Rewards API
  slug: wellnessliving-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-rewards-api-openapi.yml
- filename: wellnessliving-staff-api-openapi.yml
  format: yaml
  label: WellnessLiving Staff API
  slug: wellnessliving-staff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-staff-api-openapi.yml
- filename: wellnessliving-websocket-api-openapi.yml
  format: yaml
  label: WellnessLiving WebSocket API
  slug: wellnessliving-websocket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-websocket-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wellnessliving.com
  spf: true
hosts:
- cert_expires: Sep 21 19:39:28 2026 GMT
  host: www.wellnessliving.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: help.wellnessliving.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 19:39:28 2026 GMT
  host: us.wellnessliving.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wellnessliving Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WellnessLiving, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WellnessLiving
provider_slug: wellnessliving
slug: wellnessliving-domain-security
source_filename: wellnessliving-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wellnessliving.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 19:39:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.wellnessliving.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us.wellnessliving.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 19:39:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wellnessliving.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/security/wellnessliving-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fitness
- Wellness
- Spa
- Business Management
- Scheduling
- Memberships
- Point of Sale
---
