---
api_specs:
- filename: webflow-data-api-openapi.yml
  format: yaml
  label: Webflow Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-data-api-openapi.yml
- filename: webflow-meta-openapi.yml
  format: yaml
  label: Webflow Meta API
  slug: meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-meta-openapi.yml
- filename: webflow-sites-openapi.yml
  format: yaml
  label: Webflow Sites API
  slug: sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-sites-openapi.yml
- filename: webflow-pages-openapi.yml
  format: yaml
  label: Webflow Pages API
  slug: pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-pages-openapi.yml
- filename: webflow-collections-openapi.yml
  format: yaml
  label: Webflow Collections API
  slug: collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-collections-openapi.yml
- filename: webflow-items-openapi.yml
  format: yaml
  label: Webflow CMS Items API
  slug: items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-items-openapi.yml
- filename: webflow-components-openapi.yml
  format: yaml
  label: Webflow Components API
  slug: components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-components-openapi.yml
- filename: webflow-assets-openapi.yml
  format: yaml
  label: Webflow Assets API
  slug: assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-assets-openapi.yml
- filename: webflow-forms-openapi.yml
  format: yaml
  label: Webflow Forms API
  slug: forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-forms-openapi.yml
- filename: webflow-products-openapi.yml
  format: yaml
  label: Webflow Products and SKUs API
  slug: products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-products-openapi.yml
- filename: webflow-orders-openapi.yml
  format: yaml
  label: Webflow Orders API
  slug: orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-orders-openapi.yml
- filename: webflow-inventory-openapi.yml
  format: yaml
  label: Webflow Inventory API
  slug: inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-inventory-openapi.yml
- filename: webflow-ecommerce-settings-openapi.yml
  format: yaml
  label: Webflow Ecommerce Settings API
  slug: ecommerce-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-ecommerce-settings-openapi.yml
- filename: webflow-webhooks-openapi.yml
  format: yaml
  label: Webflow Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-webhooks-openapi.yml
- filename: webflow-custom-code-openapi.yml
  format: yaml
  label: Webflow Custom Code API
  slug: custom-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-custom-code-openapi.yml
- filename: webflow-comments-openapi.yml
  format: yaml
  label: Webflow Comments API
  slug: comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-comments-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: webflow.com
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: developers.webflow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: webflow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: api.webflow.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Webflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Webflow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Webflow
provider_slug: webflow
slug: webflow-domain-security
source_filename: webflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.webflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: webflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.webflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: webflow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/security/webflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- Ecommerce
- No-Code
- Web Development
---
