---
api_specs:
- filename: shippit-openapi.yml
  format: yaml
  label: Shippit Quote API
  slug: shippit-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/openapi/shippit-openapi.yml
- filename: shippit-openapi.yml
  format: yaml
  label: Shippit Orders API
  slug: shippit-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/openapi/shippit-openapi.yml
- filename: shippit-openapi.yml
  format: yaml
  label: Shippit Book API
  slug: shippit-book-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/openapi/shippit-openapi.yml
- filename: shippit-openapi.yml
  format: yaml
  label: Shippit Label API
  slug: shippit-label-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/openapi/shippit-openapi.yml
- filename: shippit-openapi.yml
  format: yaml
  label: Shippit Tracking API
  slug: shippit-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/openapi/shippit-openapi.yml
- filename: shippit-openapi.yml
  format: yaml
  label: Shippit Merchant API
  slug: shippit-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/openapi/shippit-openapi.yml
description: ''
domains:
- caa:
  - letsencrypt.org
  - pki.goog; cansignhttpexchanges=yes
  - amazontrust.com
  - digicert.com; cansignhttpexchanges=yes
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shippit.com
  spf: true
  spf_policy: -all
hosts:
- cert_expires: Aug 24 07:56:33 2026 GMT
  host: shippit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: app.shippit.com
  hsts: false
  https: true
  note: Root request returns a 301 redirect without an HSTS header; API base is https://app.shippit.com/api/3.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shippit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shippit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shippit
provider_slug: shippit
slug: shippit-domain-security
source_filename: shippit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + API hosts\nhosts:\n- host: shippit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 07:56:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.shippit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: false\n  note: Root request returns a 301 redirect without an HSTS header; API base is https://app.shippit.com/api/3.\ndomains:\n- domain: shippit.com\n  dnssec: false\n  caa:\n  - 'letsencrypt.org'\n  - 'pki.goog; cansignhttpexchanges=yes'\n  - 'amazontrust.com'\n  - 'digicert.com; cansignhttpexchanges=yes'\n  spf: true\n  spf_policy: '-all'\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/security/shippit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Shipping
- Logistics
- Fulfillment
- Australia
- APAC
- Multi-Carrier
- Labels
- Tracking
- Parcels
- E-commerce Logistics
- SaaS
---
