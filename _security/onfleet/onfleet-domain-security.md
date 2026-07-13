---
api_specs:
- filename: onfleet-tasks-api-openapi.yml
  format: yaml
  label: Onfleet Tasks API
  slug: onfleet-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-tasks-api-openapi.yml
- filename: onfleet-workers-api-openapi.yml
  format: yaml
  label: Onfleet Workers API
  slug: onfleet-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-workers-api-openapi.yml
- filename: onfleet-route-plans-api-openapi.yml
  format: yaml
  label: Onfleet Route Plans API
  slug: onfleet-route-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-route-plans-api-openapi.yml
- filename: onfleet-orders-api-openapi.yml
  format: yaml
  label: Onfleet Orders API
  slug: onfleet-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-orders-api-openapi.yml
- filename: onfleet-organizations-api-openapi.yml
  format: yaml
  label: Onfleet Organizations & Teams API
  slug: onfleet-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-organizations-api-openapi.yml
- filename: onfleet-recipients-api-openapi.yml
  format: yaml
  label: Onfleet Recipients API
  slug: onfleet-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-recipients-api-openapi.yml
- filename: onfleet-destinations-api-openapi.yml
  format: yaml
  label: Onfleet Destinations API
  slug: onfleet-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-destinations-api-openapi.yml
- filename: onfleet-webhooks-api-openapi.yml
  format: yaml
  label: Onfleet Webhooks API
  slug: onfleet-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:devops+caa@onfleet.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: onfleet.com
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: onfleet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 15:15:35 2026 GMT
  host: docs.onfleet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onfleet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Onfleet, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Onfleet
provider_slug: onfleet
slug: onfleet-domain-security
source_filename: onfleet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onfleet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.onfleet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:15:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: onfleet.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:devops+caa@onfleet.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/security/onfleet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Last Mile Delivery
- Logistics
- Fleet Management
- Dispatch
- Route Optimization
- Courier
- Drivers
- Tracking
- Geocoding
- Webhooks
- AI
- SaaS
---
