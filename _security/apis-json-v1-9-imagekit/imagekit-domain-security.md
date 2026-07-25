---
api_specs:
- filename: imagekit-account-management-api-api-openapi.yml
  format: yaml
  label: ImageKit Account Management API API
  slug: imagekit-account-management-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-account-management-api-api-openapi.yml
- filename: imagekit-caching-api-openapi.yml
  format: yaml
  label: ImageKit Caching API
  slug: imagekit-caching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-caching-api-openapi.yml
- filename: imagekit-custom-metadata-fields-api-openapi.yml
  format: yaml
  label: ImageKit Custom metadata fields API
  slug: imagekit-custom-metadata-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-custom-metadata-fields-api-openapi.yml
- filename: imagekit-digital-asset-management-dam-api-openapi.yml
  format: yaml
  label: ImageKit Digital Asset Management (DAM) API
  slug: imagekit-digital-asset-management-dam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-digital-asset-management-dam-api-openapi.yml
- filename: imagekit-dummy-test-api-openapi.yml
  format: yaml
  label: ImageKit Dummy Test API
  slug: imagekit-dummy-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-dummy-test-api-openapi.yml
- filename: imagekit-file-metadata-api-openapi.yml
  format: yaml
  label: ImageKit File Metadata API
  slug: imagekit-file-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-file-metadata-api-openapi.yml
- filename: imagekit-managing-assets-api-openapi.yml
  format: yaml
  label: ImageKit Managing assets API
  slug: imagekit-managing-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-managing-assets-api-openapi.yml
- filename: imagekit-managing-folders-api-openapi.yml
  format: yaml
  label: ImageKit Managing folders API
  slug: imagekit-managing-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-managing-folders-api-openapi.yml
- filename: imagekit-origins-api-openapi.yml
  format: yaml
  label: ImageKit Origins API
  slug: imagekit-origins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-origins-api-openapi.yml
- filename: imagekit-saved-extensions-api-openapi.yml
  format: yaml
  label: ImageKit Saved Extensions API
  slug: imagekit-saved-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-saved-extensions-api-openapi.yml
- filename: imagekit-upload-file-api-openapi.yml
  format: yaml
  label: ImageKit Upload File API
  slug: imagekit-upload-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-upload-file-api-openapi.yml
- filename: imagekit-url-endpoints-api-openapi.yml
  format: yaml
  label: ImageKit URL endpoints API
  slug: imagekit-url-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-url-endpoints-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: imagekit.io
  spf: true
hosts:
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: imagekit.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 23:59:59 2026 GMT
  host: api.imagekit.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imagekit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ImageKit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ImageKit
provider_slug: apis-json-v1-9-imagekit
slug: imagekit-domain-security
source_filename: imagekit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imagekit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.imagekit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: imagekit.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/security/imagekit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Images
- Video
- CDN
- Media
- Optimization
- Transformations
- Digital Asset Management
- DAM
- Storage
- Cache
- Upload
---
