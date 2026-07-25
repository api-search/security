---
api_specs:
- filename: adobe-photoshop-actions-api-openapi.yml
  format: yaml
  label: Adobe Photoshop Actions API
  slug: adobe-photoshop-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/openapi/adobe-photoshop-actions-api-openapi.yml
- filename: adobe-photoshop-background-removal-api-openapi.yml
  format: yaml
  label: Adobe Photoshop Background Removal API
  slug: adobe-photoshop-background-removal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/openapi/adobe-photoshop-background-removal-api-openapi.yml
- filename: adobe-photoshop-crop-and-effects-api-openapi.yml
  format: yaml
  label: Adobe Photoshop Crop and Effects API
  slug: adobe-photoshop-crop-and-effects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/openapi/adobe-photoshop-crop-and-effects-api-openapi.yml
- filename: adobe-photoshop-document-operations-api-openapi.yml
  format: yaml
  label: Adobe Photoshop Document Operations API
  slug: adobe-photoshop-document-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/openapi/adobe-photoshop-document-operations-api-openapi.yml
- filename: adobe-photoshop-generative-api-openapi.yml
  format: yaml
  label: Adobe Photoshop Generative API
  slug: adobe-photoshop-generative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/openapi/adobe-photoshop-generative-api-openapi.yml
- filename: adobe-photoshop-health-api-openapi.yml
  format: yaml
  label: Adobe Photoshop Health API
  slug: adobe-photoshop-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/openapi/adobe-photoshop-health-api-openapi.yml
- filename: adobe-photoshop-renditions-api-openapi.yml
  format: yaml
  label: Adobe Photoshop Renditions API
  slug: adobe-photoshop-renditions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/openapi/adobe-photoshop-renditions-api-openapi.yml
- filename: adobe-photoshop-smart-objects-api-openapi.yml
  format: yaml
  label: Adobe Photoshop Smart Objects API
  slug: adobe-photoshop-smart-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/openapi/adobe-photoshop-smart-objects-api-openapi.yml
- filename: adobe-photoshop-status-api-openapi.yml
  format: yaml
  label: Adobe Photoshop Status API
  slug: adobe-photoshop-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/openapi/adobe-photoshop-status-api-openapi.yml
- filename: adobe-photoshop-text-api-openapi.yml
  format: yaml
  label: Adobe Photoshop Text API
  slug: adobe-photoshop-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/openapi/adobe-photoshop-text-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.io
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: developer.adobe.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: www.adobe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: image.adobe.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adobe Photoshop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adobe Photoshop, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adobe Photoshop
provider_slug: adobe-photoshop
slug: adobe-photoshop-domain-security
source_filename: adobe-photoshop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.adobe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: www.adobe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\n- host: image.adobe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: adobe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: adobe.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/security/adobe-photoshop-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- AI/ML
- Creative Cloud
- Image Editing
- Photoshop
- Plugins
- REST API
- Scripting
---
