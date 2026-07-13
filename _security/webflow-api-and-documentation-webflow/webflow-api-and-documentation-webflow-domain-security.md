---
api_specs:
- filename: webflow-data-api-openapi.yml
  format: yaml
  label: Webflow Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow-api-and-documentation-webflow/refs/heads/main/openapi/webflow-data-api-openapi.yml
- filename: webflow-sites-openapi.yml
  format: yaml
  label: Webflow Sites API
  slug: sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow-api-and-documentation-webflow/refs/heads/main/openapi/webflow-sites-openapi.yml
- filename: webflow-collections-openapi.yml
  format: yaml
  label: Webflow Collections API
  slug: collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow-api-and-documentation-webflow/refs/heads/main/openapi/webflow-collections-openapi.yml
- filename: webflow-items-openapi.yml
  format: yaml
  label: Webflow CMS Items API
  slug: items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow-api-and-documentation-webflow/refs/heads/main/openapi/webflow-items-openapi.yml
- filename: webflow-webhooks-openapi.yml
  format: yaml
  label: Webflow Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow-api-and-documentation-webflow/refs/heads/main/openapi/webflow-webhooks-openapi.yml
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
name: Webflow Api And Documentation Webflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Webflow API and Documentation, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Webflow API and Documentation
provider_slug: webflow-api-and-documentation-webflow
slug: webflow-api-and-documentation-webflow-domain-security
source_filename: webflow-api-and-documentation-webflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.webflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: webflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.webflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: webflow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webflow-api-and-documentation-webflow/refs/heads/main/security/webflow-api-and-documentation-webflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- Content Management
- Ecommerce
- No-Code
- Publishing
- Web Development
---
