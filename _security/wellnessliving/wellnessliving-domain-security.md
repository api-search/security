---
api_specs:
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Clients API
  slug: clients
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Classes & Schedules API
  slug: classes-schedule
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Appointments API
  slug: appointments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Booking Wizard API
  slug: booking-wizard
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Memberships & Passes API
  slug: memberships-passes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Staff API
  slug: staff
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Locations API
  slug: locations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Business API
  slug: business
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Sales & Catalog API
  slug: sales-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Authentication API
  slug: authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Rewards & Loyalty API
  slug: rewards-loyalty
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Reviews API
  slug: reviews
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Reports API
  slug: reports
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Real-Time Notifications API
  slug: realtime-notifications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
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
