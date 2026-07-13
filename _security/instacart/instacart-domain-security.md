---
api_specs:
- filename: instacart-developer-platform-api-openapi.yml
  format: yaml
  label: Instacart Developer Platform API
  slug: developer-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-developer-platform-api-openapi.yml
- filename: instacart-connect-fulfillment-api-openapi.yml
  format: yaml
  label: Instacart Connect Fulfillment API
  slug: connect-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-connect-fulfillment-api-openapi.yml
- filename: instacart-connect-post-checkout-api-openapi.yml
  format: yaml
  label: Instacart Connect Post-Checkout API
  slug: connect-post-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-connect-post-checkout-api-openapi.yml
- filename: instacart-catalog-api-openapi.yml
  format: yaml
  label: Instacart Catalog API
  slug: catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-catalog-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: instacart.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: instacart.tools
  spf: true
hosts:
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: docs.instacart.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: connect.instacart.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: connect.dev.instacart.tools
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instacart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for instacart, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: instacart
provider_slug: instacart
slug: instacart-domain-security
source_filename: instacart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.instacart.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: false\n- host: connect.instacart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\n- host: connect.dev.instacart.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: instacart.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: instacart.tools\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/security/instacart-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags: []
---
