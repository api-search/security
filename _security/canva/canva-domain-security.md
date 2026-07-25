---
api_specs:
- filename: canva-assets-api-openapi.yml
  format: yaml
  label: Canva Assets API
  slug: canva-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-assets-api-openapi.yml
- filename: canva-autofills-api-openapi.yml
  format: yaml
  label: Canva Autofills API
  slug: canva-autofills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-autofills-api-openapi.yml
- filename: canva-brand-templates-api-openapi.yml
  format: yaml
  label: Canva Brand Templates API
  slug: canva-brand-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-brand-templates-api-openapi.yml
- filename: canva-comments-api-openapi.yml
  format: yaml
  label: Canva Comments API
  slug: canva-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-comments-api-openapi.yml
- filename: canva-designs-api-openapi.yml
  format: yaml
  label: Canva Designs API
  slug: canva-designs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-designs-api-openapi.yml
- filename: canva-exports-api-openapi.yml
  format: yaml
  label: Canva Exports API
  slug: canva-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-exports-api-openapi.yml
- filename: canva-folders-api-openapi.yml
  format: yaml
  label: Canva Folders API
  slug: canva-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-folders-api-openapi.yml
- filename: canva-resizes-api-openapi.yml
  format: yaml
  label: Canva Resizes API
  slug: canva-resizes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-resizes-api-openapi.yml
- filename: canva-users-api-openapi.yml
  format: yaml
  label: Canva Users API
  slug: canva-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: canva.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: canva.dev
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: www.canva.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: api.canva.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 07:04:18 2026 GMT
  host: www.canva.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Canva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canva, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Canva
provider_slug: canva
slug: canva-domain-security
source_filename: canva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.canva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.canva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\n- host: www.canva.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 07:04:18 2026 GMT\n  hsts: null\ndomains:\n- domain: canva.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: canva.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/security/canva-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Apps
- Automation
- Brand Management
- Collaboration
- Design
- Graphics
- Marketing
- Print
- Templates
- Visual Content
---
