---
api_specs:
- filename: teelaunch-openapi.yml
  format: yaml
  label: Teelaunch Account API
  slug: teelaunch-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-openapi.yml
- filename: teelaunch-openapi.yml
  format: yaml
  label: Teelaunch Blank Catalog API
  slug: teelaunch-blank-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-openapi.yml
- filename: teelaunch-openapi.yml
  format: yaml
  label: Teelaunch Products API
  slug: teelaunch-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-openapi.yml
- filename: teelaunch-openapi.yml
  format: yaml
  label: Teelaunch Orders API
  slug: teelaunch-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-openapi.yml
- filename: teelaunch-openapi.yml
  format: yaml
  label: Teelaunch Shipping & Tracking API
  slug: teelaunch-shipping-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-openapi.yml
- filename: teelaunch-openapi.yml
  format: yaml
  label: Teelaunch Platforms & Stores API
  slug: teelaunch-platforms-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: teelaunch.com
  spf: true
hosts:
- cert_expires: Sep 19 08:07:53 2026 GMT
  host: teelaunch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 08:07:53 2026 GMT
  host: api.teelaunch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teelaunch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teelaunch, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Teelaunch
provider_slug: teelaunch
slug: teelaunch-domain-security
source_filename: teelaunch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teelaunch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 08:07:53 2026 GMT\n  hsts: false\n- host: api.teelaunch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 08:07:53 2026 GMT\n  hsts: false\ndomains:\n- domain: teelaunch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/security/teelaunch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Print on Demand
- POD
- Ecommerce
- Fulfillment
- Dropshipping
- Orders
- Shipping
---
