---
api_specs:
- filename: storyblok-webhooks-asyncapi.yml
  format: yaml
  label: Storyblok Webhooks
  slug: storyblok-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/asyncapi/storyblok-webhooks-asyncapi.yml
- filename: storyblok-assets-api-openapi.yml
  format: yaml
  label: Storyblok Assets API
  slug: storyblok-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/openapi/storyblok-assets-api-openapi.yml
- filename: storyblok-collaborators-api-openapi.yml
  format: yaml
  label: Storyblok Collaborators API
  slug: storyblok-collaborators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/openapi/storyblok-collaborators-api-openapi.yml
- filename: storyblok-components-api-openapi.yml
  format: yaml
  label: Storyblok Components API
  slug: storyblok-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/openapi/storyblok-components-api-openapi.yml
- filename: storyblok-datasources-api-openapi.yml
  format: yaml
  label: Storyblok Datasources API
  slug: storyblok-datasources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/openapi/storyblok-datasources-api-openapi.yml
- filename: storyblok-image-transformation-api-openapi.yml
  format: yaml
  label: Storyblok Image Transformation API
  slug: storyblok-image-transformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/openapi/storyblok-image-transformation-api-openapi.yml
- filename: storyblok-links-api-openapi.yml
  format: yaml
  label: Storyblok Links API
  slug: storyblok-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/openapi/storyblok-links-api-openapi.yml
- filename: storyblok-spaces-api-openapi.yml
  format: yaml
  label: Storyblok Spaces API
  slug: storyblok-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/openapi/storyblok-spaces-api-openapi.yml
- filename: storyblok-stories-api-openapi.yml
  format: yaml
  label: Storyblok Stories API
  slug: storyblok-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/openapi/storyblok-stories-api-openapi.yml
- filename: storyblok-tags-api-openapi.yml
  format: yaml
  label: Storyblok Tags API
  slug: storyblok-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/openapi/storyblok-tags-api-openapi.yml
- filename: storyblok-webhooks-api-openapi.yml
  format: yaml
  label: Storyblok Webhooks API
  slug: storyblok-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/openapi/storyblok-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: storyblok.com
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: www.storyblok.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: api.storyblok.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: mapi.storyblok.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Storyblok Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Storyblok, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Storyblok
provider_slug: storyblok
slug: storyblok-domain-security
source_filename: storyblok-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.storyblok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.storyblok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: false\n- host: mapi.storyblok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: storyblok.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/security/storyblok-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- Content Delivery
- Content Management
- Headless CMS
- Image Optimization
- REST API
- Visual Editor
- Webhook
---
