---
api_specs:
- filename: omnisend-analytics-api-openapi.yml
  format: yaml
  label: Omnisend Analytics API
  slug: omnisend-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-analytics-api-openapi.yml
- filename: omnisend-batches-api-openapi.yml
  format: yaml
  label: Omnisend Batches API
  slug: omnisend-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-batches-api-openapi.yml
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
- filename: omnisend-emailcontent-api-openapi.yml
  format: yaml
  label: Omnisend EmailContent API
  slug: omnisend-emailcontent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-emailcontent-api-openapi.yml
- filename: omnisend-emailtemplates-api-openapi.yml
  format: yaml
  label: Omnisend EmailTemplates API
  slug: omnisend-emailtemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-emailtemplates-api-openapi.yml
- filename: omnisend-emailuniversallayouts-api-openapi.yml
  format: yaml
  label: Omnisend EmailUniversalLayouts API
  slug: omnisend-emailuniversallayouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-emailuniversallayouts-api-openapi.yml
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
- filename: omnisend-productcategories-api-openapi.yml
  format: yaml
  label: Omnisend ProductCategories API
  slug: omnisend-productcategories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-productcategories-api-openapi.yml
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
