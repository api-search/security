---
api_specs:
- filename: doctofam-com-appointments-api-openapi.yml
  format: yaml
  label: Doctofam Appointments API
  slug: doctofam-com-appointments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-appointments-api-openapi.yml
- filename: doctofam-com-clinics-api-openapi.yml
  format: yaml
  label: Doctofam Clinics API
  slug: doctofam-com-clinics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-clinics-api-openapi.yml
- filename: doctofam-com-invoices-api-openapi.yml
  format: yaml
  label: Doctofam Invoices API
  slug: doctofam-com-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-invoices-api-openapi.yml
- filename: doctofam-com-patients-api-openapi.yml
  format: yaml
  label: Doctofam Patients API
  slug: doctofam-com-patients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-patients-api-openapi.yml
- filename: doctofam-com-payments-api-openapi.yml
  format: yaml
  label: Doctofam Payments API
  slug: doctofam-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-payments-api-openapi.yml
- filename: doctofam-com-procedures-api-openapi.yml
  format: yaml
  label: Doctofam Procedures API
  slug: doctofam-com-procedures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-procedures-api-openapi.yml
- filename: doctofam-com-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Doctofam Webhook subscriptions API
  slug: doctofam-com-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-webhook-subscriptions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: doctofam.com
  spf: true
hosts:
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: doctofam.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Doctofam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Doctofam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Doctofam
provider_slug: doctofam-com
slug: doctofam-com-domain-security
source_filename: doctofam-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doctofam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: doctofam.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/doctofam-com/security/doctofam-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Medical Practice Management
- Appointment Scheduling
- Billing and Insurance
---
