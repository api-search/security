---
api_specs:
- filename: einride-authenticationservice-api-openapi.yml
  format: yaml
  label: Einride AuthenticationService API
  slug: einride-authenticationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/einride/refs/heads/main/openapi/einride-authenticationservice-api-openapi.yml
- filename: einride-bookingservice-api-openapi.yml
  format: yaml
  label: Einride BookingService API
  slug: einride-bookingservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/einride/refs/heads/main/openapi/einride-bookingservice-api-openapi.yml
- filename: einride-shipmentservice-api-openapi.yml
  format: yaml
  label: Einride ShipmentService API
  slug: einride-shipmentservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/einride/refs/heads/main/openapi/einride-shipmentservice-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: einride.tech
  spf: true
hosts:
- cert_expires: Aug 23 18:40:41 2026 GMT
  host: www.einride.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Einride Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Einride, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Einride
provider_slug: einride
slug: einride-domain-security
source_filename: einride-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.einride.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 18:40:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: einride.tech\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/einride/refs/heads/main/security/einride-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sustainable Transport
- Freight
- Logistics
- Autonomous Vehicles
- Electric Vehicles
- Shipping
- gRPC
- Sweden
---
