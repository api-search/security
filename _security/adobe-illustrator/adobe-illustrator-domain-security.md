---
api_specs:
- filename: adobe-illustrator-application-api-openapi.yml
  format: yaml
  label: Adobe Illustrator Application API
  slug: adobe-illustrator-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/openapi/adobe-illustrator-application-api-openapi.yml
- filename: adobe-illustrator-artboards-api-openapi.yml
  format: yaml
  label: Adobe Illustrator Artboards API
  slug: adobe-illustrator-artboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/openapi/adobe-illustrator-artboards-api-openapi.yml
- filename: adobe-illustrator-documents-api-openapi.yml
  format: yaml
  label: Adobe Illustrator Documents API
  slug: adobe-illustrator-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/openapi/adobe-illustrator-documents-api-openapi.yml
- filename: adobe-illustrator-graphic-styles-api-openapi.yml
  format: yaml
  label: Adobe Illustrator Graphic Styles API
  slug: adobe-illustrator-graphic-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/openapi/adobe-illustrator-graphic-styles-api-openapi.yml
- filename: adobe-illustrator-layers-api-openapi.yml
  format: yaml
  label: Adobe Illustrator Layers API
  slug: adobe-illustrator-layers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/openapi/adobe-illustrator-layers-api-openapi.yml
- filename: adobe-illustrator-path-items-api-openapi.yml
  format: yaml
  label: Adobe Illustrator Path Items API
  slug: adobe-illustrator-path-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/openapi/adobe-illustrator-path-items-api-openapi.yml
- filename: adobe-illustrator-swatches-api-openapi.yml
  format: yaml
  label: Adobe Illustrator Swatches API
  slug: adobe-illustrator-swatches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/openapi/adobe-illustrator-swatches-api-openapi.yml
- filename: adobe-illustrator-symbols-api-openapi.yml
  format: yaml
  label: Adobe Illustrator Symbols API
  slug: adobe-illustrator-symbols-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/openapi/adobe-illustrator-symbols-api-openapi.yml
- filename: adobe-illustrator-text-frames-api-openapi.yml
  format: yaml
  label: Adobe Illustrator Text Frames API
  slug: adobe-illustrator-text-frames-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/openapi/adobe-illustrator-text-frames-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.com
  spf: true
hosts:
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: www.adobe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: developer.adobe.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Adobe Illustrator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adobe Illustrator, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adobe Illustrator
provider_slug: adobe-illustrator
slug: adobe-illustrator-domain-security
source_filename: adobe-illustrator-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adobe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\n- host: developer.adobe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: adobe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-illustrator/refs/heads/main/security/adobe-illustrator-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Creative Cloud
- Design
- Illustrator
- Vector Graphics
---
