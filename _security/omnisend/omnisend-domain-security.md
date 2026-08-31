---
api_specs:
- filename: omnisend-brands-api-openapi.yml
  format: yaml
  label: Omnisend Brands API
  slug: omnisend-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-brands-api-openapi.yml
- filename: omnisend-campaigns-api-openapi.yml
  format: yaml
  label: Omnisend Campaigns API
  slug: omnisend-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-campaigns-api-openapi.yml
- filename: omnisend-contacts-api-openapi.yml
  format: yaml
  label: Omnisend Contacts API
  slug: omnisend-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-contacts-api-openapi.yml
- filename: omnisend-events-api-openapi.yml
  format: yaml
  label: Omnisend Events API
  slug: omnisend-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-events-api-openapi.yml
- filename: omnisend-images-api-openapi.yml
  format: yaml
  label: Omnisend Images API
  slug: omnisend-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-images-api-openapi.yml
- filename: omnisend-products-api-openapi.yml
  format: yaml
  label: Omnisend Products API
  slug: omnisend-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-products-api-openapi.yml
- filename: omnisend-segments-api-openapi.yml
  format: yaml
  label: Omnisend Segments API
  slug: omnisend-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-segments-api-openapi.yml
- filename: omnisend-automations-api-openapi.yml
  format: yaml
  label: Omnisend Automations API
  slug: omnisend-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-automations-api-openapi.yml
- filename: omnisend-event-metadata-api-openapi.yml
  format: yaml
  label: Omnisend Event Metadata API
  slug: omnisend-event-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-event-metadata-api-openapi.yml
- filename: omnisend-batch-api-openapi.yml
  format: yaml
  label: Omnisend Batch API
  slug: omnisend-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-batch-api-openapi.yml
- filename: omnisend-email-content-api-openapi.yml
  format: yaml
  label: Omnisend Email Content API
  slug: omnisend-email-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-email-content-api-openapi.yml
- filename: omnisend-email-templates-api-openapi.yml
  format: yaml
  label: Omnisend Email Templates API
  slug: omnisend-email-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-email-templates-api-openapi.yml
- filename: omnisend-email-universal-layouts-api-openapi.yml
  format: yaml
  label: Omnisend Email Universal Layouts API
  slug: omnisend-email-universal-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-email-universal-layouts-api-openapi.yml
- filename: omnisend-product-categories-api-openapi.yml
  format: yaml
  label: Omnisend Product Categories API
  slug: omnisend-product-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-product-categories-api-openapi.yml
- filename: omnisend-reports-api-openapi.yml
  format: yaml
  label: Omnisend Reports API
  slug: omnisend-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-reports-api-openapi.yml
- filename: omnisend-statistics-api-openapi.yml
  format: yaml
  label: Omnisend Statistics API
  slug: omnisend-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-statistics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: omnisend.com
  spf: true
hosts:
- cert_expires: Sep 28 23:48:03 2026 GMT
  host: www.omnisend.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 19:25:10 2026 GMT
  host: api-docs.omnisend.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 15:28:18 2026 GMT
  host: api.omnisend.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Omnisend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Omnisend, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Omnisend
provider_slug: omnisend
slug: omnisend-domain-security
source_filename: omnisend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.omnisend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:48:03 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api-docs.omnisend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:25:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.omnisend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 15:28:18 2026 GMT\n  hsts: null\ndomains:\n- domain: omnisend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/security/omnisend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Marketing
- Marketing Automation
- E-Commerce
- SMS Marketing
- Customer Engagement
- Segmentation
- Campaigns
- Forms
- Popups
- Web Push
- Automation Workflows
- Analytics
- MCP
- Agent Ready
- Transactional Messaging
---
