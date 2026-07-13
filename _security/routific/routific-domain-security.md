---
api_specs:
- filename: routific-route-optimization-api-openapi.yml
  format: yaml
  label: Routific Route Optimization API
  slug: routific-route-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routific/refs/heads/main/openapi/routific-route-optimization-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  - 0 iodef "mailto:devs@routific.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: routific.com
  spf: true
hosts:
- cert_expires: Aug 17 22:02:04 2026 GMT
  host: routific.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 06:54:35 2026 GMT
  host: docs.routific.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 23:10:31 2026 GMT
  host: api.routific.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Routific Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Routific, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Routific
provider_slug: routific
slug: routific-domain-security
source_filename: routific-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: routific.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 22:02:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.routific.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 06:54:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.routific.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 23:10:31 2026 GMT\n  hsts: null\ndomains:\n- domain: routific.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 0 iodef \"mailto:devs@routific.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/routific/refs/heads/main/security/routific-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- RouteOptimization
- VRP
- PickupAndDelivery
- Logistics
- LastMileDelivery
- Delivery
- FleetManagement
- Dispatch
- DeliveryManagement
---
