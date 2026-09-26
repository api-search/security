---
api_specs:
- filename: agendapro-available-slots-api-openapi.yml
  format: yaml
  label: AgendaPro Available Slots API
  slug: agendapro-available-slots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-available-slots-api-openapi.yml
- filename: agendapro-bookings-api-openapi.yml
  format: yaml
  label: AgendaPro Bookings API
  slug: agendapro-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-bookings-api-openapi.yml
- filename: agendapro-carts-api-openapi.yml
  format: yaml
  label: AgendaPro Carts API
  slug: agendapro-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-carts-api-openapi.yml
- filename: agendapro-clients-api-openapi.yml
  format: yaml
  label: AgendaPro Clients API
  slug: agendapro-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-clients-api-openapi.yml
- filename: agendapro-custom-attributes-api-openapi.yml
  format: yaml
  label: AgendaPro Custom Attributes API
  slug: agendapro-custom-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-custom-attributes-api-openapi.yml
- filename: agendapro-locations-api-openapi.yml
  format: yaml
  label: AgendaPro Locations API
  slug: agendapro-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-locations-api-openapi.yml
- filename: agendapro-payment-requests-api-openapi.yml
  format: yaml
  label: AgendaPro Payment Requests API
  slug: agendapro-payment-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-payment-requests-api-openapi.yml
- filename: agendapro-providers-api-openapi.yml
  format: yaml
  label: AgendaPro Providers API
  slug: agendapro-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-providers-api-openapi.yml
- filename: agendapro-sales-api-openapi.yml
  format: yaml
  label: AgendaPro Sales API
  slug: agendapro-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-sales-api-openapi.yml
- filename: agendapro-services-api-openapi.yml
  format: yaml
  label: AgendaPro Services API
  slug: agendapro-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-services-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: agendapro.com
  spf: true
hosts:
- cert_expires: Oct 26 08:31:57 2026 GMT
  host: agendapro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 06:23:20 2026 GMT
  host: developers.agendapro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: connect.agendapro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Agendapro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgendaPro, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AgendaPro
provider_slug: agendapro
slug: agendapro-domain-security
source_filename: agendapro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agendapro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 08:31:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.agendapro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 06:23:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: connect.agendapro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: agendapro.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/security/agendapro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Appointment Scheduling
- Booking
- Salon Software
- Spa and Wellness
- Point-of-Sale
- Clinic Management
- CRM
- Payments
- Webhook
- Vertical SaaS
- Latin America
- Small Business
- Scheduling
---
