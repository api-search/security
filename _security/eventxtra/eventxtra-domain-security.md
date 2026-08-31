---
api_specs:
- filename: eventxtra-attendee-api-openapi.yml
  format: yaml
  label: EventX Attendee API
  slug: eventxtra-attendee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-attendee-api-openapi.yml
- filename: eventxtra-auth-api-openapi.yml
  format: yaml
  label: EventX Auth API
  slug: eventxtra-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-auth-api-openapi.yml
- filename: eventxtra-custom-field-api-openapi.yml
  format: yaml
  label: EventX Custom Field API
  slug: eventxtra-custom-field-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-custom-field-api-openapi.yml
- filename: eventxtra-event-api-openapi.yml
  format: yaml
  label: EventX Event API
  slug: eventxtra-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-event-api-openapi.yml
- filename: eventxtra-event-webhook-api-openapi.yml
  format: yaml
  label: EventX Event Webhook API
  slug: eventxtra-event-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-event-webhook-api-openapi.yml
- filename: eventxtra-invoice-api-openapi.yml
  format: yaml
  label: EventX Invoice API
  slug: eventxtra-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-invoice-api-openapi.yml
- filename: eventxtra-media-api-openapi.yml
  format: yaml
  label: EventX Media API
  slug: eventxtra-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-media-api-openapi.yml
- filename: eventxtra-order-api-openapi.yml
  format: yaml
  label: EventX Order API
  slug: eventxtra-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-order-api-openapi.yml
- filename: eventxtra-outreach-api-openapi.yml
  format: yaml
  label: EventX Outreach API
  slug: eventxtra-outreach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-outreach-api-openapi.yml
- filename: eventxtra-public-api-api-openapi.yml
  format: yaml
  label: EventX Public API
  slug: eventxtra-public-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-public-api-api-openapi.yml
- filename: eventxtra-registration-form-api-openapi.yml
  format: yaml
  label: EventX Registration Form API
  slug: eventxtra-registration-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-registration-form-api-openapi.yml
- filename: eventxtra-registration-order-api-openapi.yml
  format: yaml
  label: EventX Registration Order API
  slug: eventxtra-registration-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-registration-order-api-openapi.yml
- filename: eventxtra-registration-service-api-openapi.yml
  format: yaml
  label: EventX Registration Service API
  slug: eventxtra-registration-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-registration-service-api-openapi.yml
- filename: eventxtra-salesforce-api-openapi.yml
  format: yaml
  label: EventX Salesforce API
  slug: eventxtra-salesforce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-salesforce-api-openapi.yml
- filename: eventxtra-ticket-class-api-openapi.yml
  format: yaml
  label: EventX Ticket Class API
  slug: eventxtra-ticket-class-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-ticket-class-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eventx.io
  spf: true
hosts:
- cert_expires: Sep 23 09:17:33 2026 GMT
  host: eventx.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 13:48:04 2026 GMT
  host: esaas-api.eventx.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eventxtra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EventX, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: EventX
provider_slug: eventxtra
slug: eventxtra-domain-security
source_filename: eventxtra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eventx.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 09:17:33 2026 GMT\n  hsts: false\n- host: esaas-api.eventx.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 13:48:04 2026 GMT\n  hsts: null\ndomains:\n- domain: eventx.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/security/eventxtra-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Event Management
- Event Registration
- Ticketing
- Check-in
- Event Marketing
- Virtual Events
- Webhook
- OpenAPI
- MCP
- Artificial Intelligence
- Hong Kong
- APAC
---
