---
api_specs:
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Customers API
  slug: servicefusion-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Contacts API
  slug: servicefusion-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Jobs API
  slug: servicefusion-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Estimates API
  slug: servicefusion-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Invoices API
  slug: servicefusion-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Products and Services API
  slug: servicefusion-products-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Payments API
  slug: servicefusion-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Techs and Users API
  slug: servicefusion-techs-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Calendar Tasks API
  slug: servicefusion-calendar-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: servicefusion.com
  spf: true
hosts:
- cert_expires: Sep 14 22:39:47 2026 GMT
  host: www.servicefusion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: docs.servicefusion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: api.servicefusion.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Servicefusion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Service Fusion, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Service Fusion
provider_slug: servicefusion
slug: servicefusion-domain-security
source_filename: servicefusion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.servicefusion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 22:39:47 2026 GMT\n  hsts: false\n- host: docs.servicefusion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\n- host: api.servicefusion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: servicefusion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/security/servicefusion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Field Service Management
- FSM
- Home Services
- Contractors
- Scheduling
- Dispatch
- Invoicing
---
