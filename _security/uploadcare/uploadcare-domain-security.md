---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Uploadcare REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://uploadcare.com/api-refs/rest-api/v0.7.0/
- filename: openapi.yaml
  format: yaml
  label: Uploadcare Upload API
  slug: upload-api
  spec_type: OpenAPI
  url: https://uploadcare.com/api-refs/upload-api/
- filename: uploadcare-cdn-api-openapi.yml
  format: yaml
  label: Uploadcare CDN & Image Transformation API
  slug: cdn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uploadcare/refs/heads/main/openapi/uploadcare-cdn-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uploadcare.com
  spf: true
hosts:
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: uploadcare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: api.uploadcare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: upload.uploadcare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uploadcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uploadcare, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Uploadcare
provider_slug: uploadcare
slug: uploadcare-domain-security
source_filename: uploadcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uploadcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: false\n- host: api.uploadcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: null\n- host: upload.uploadcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: uploadcare.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uploadcare/refs/heads/main/security/uploadcare-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- File Upload
- File Management
- CDN
- Image Transformation
- Document Conversion
- Video Encoding
- Malware Scanning
- Storage
- Webhooks
---
