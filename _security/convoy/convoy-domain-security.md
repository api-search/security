---
api_specs:
- filename: convoy-delivery-attempts-api-openapi.yml
  format: yaml
  label: Convoy Delivery Attempts API
  slug: convoy-delivery-attempts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-delivery-attempts-api-openapi.yml
- filename: convoy-endpoints-api-openapi.yml
  format: yaml
  label: Convoy Endpoints API
  slug: convoy-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-endpoints-api-openapi.yml
- filename: convoy-event-deliveries-api-openapi.yml
  format: yaml
  label: Convoy Event Deliveries API
  slug: convoy-event-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-event-deliveries-api-openapi.yml
- filename: convoy-events-api-openapi.yml
  format: yaml
  label: Convoy Events API
  slug: convoy-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-events-api-openapi.yml
- filename: convoy-eventtypes-api-openapi.yml
  format: yaml
  label: Convoy EventTypes API
  slug: convoy-eventtypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-eventtypes-api-openapi.yml
- filename: convoy-filters-api-openapi.yml
  format: yaml
  label: Convoy Filters API
  slug: convoy-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-filters-api-openapi.yml
- filename: convoy-meta-events-api-openapi.yml
  format: yaml
  label: Convoy Meta Events API
  slug: convoy-meta-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-meta-events-api-openapi.yml
- filename: convoy-onboard-api-openapi.yml
  format: yaml
  label: Convoy Onboard API
  slug: convoy-onboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-onboard-api-openapi.yml
- filename: convoy-portal-links-api-openapi.yml
  format: yaml
  label: Convoy Portal Links API
  slug: convoy-portal-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-portal-links-api-openapi.yml
- filename: convoy-sources-api-openapi.yml
  format: yaml
  label: Convoy Sources API
  slug: convoy-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-sources-api-openapi.yml
- filename: convoy-subscriptions-api-openapi.yml
  format: yaml
  label: Convoy Subscriptions API
  slug: convoy-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-subscriptions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getconvoy.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getconvoy.cloud
  spf: false
hosts:
- cert_expires: Sep  4 19:29:03 2026 GMT
  host: getconvoy.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 05:54:31 2026 GMT
  host: us.getconvoy.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 18:05:48 2026 GMT
  host: eu.getconvoy.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Convoy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Convoy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Convoy
provider_slug: convoy
slug: convoy-domain-security
source_filename: convoy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getconvoy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 19:29:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: us.getconvoy.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:54:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eu.getconvoy.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 18:05:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getconvoy.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: getconvoy.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/security/convoy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Webhook
- Webhook Gateway
- Event Delivery
- Eventing
- Messaging
- Integration
- API Infrastructure
---
