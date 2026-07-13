---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Adobe Photoshop API
  slug: adobe-photoshop-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/photoshop/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Adobe Lightroom API
  slug: adobe-lightroom-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/lightroom/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Adobe PDF Services API
  slug: adobe-pdf-services-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/document-services/docs/apis/
- filename: openapi.yaml
  format: yaml
  label: Adobe PDF Extract API
  slug: adobe-pdf-extract-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/document-services/docs/apis/
- filename: openapi.yaml
  format: yaml
  label: Adobe PDF Accessibility Auto-Tag API
  slug: adobe-pdf-accessibility-auto-tag-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/document-services/docs/apis/
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
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: image.adobe.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 23:59:59 2026 GMT
  host: lr.adobe.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adobe Suite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adobe Suite, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adobe Suite
provider_slug: adobe-suite
slug: adobe-suite-domain-security
source_filename: adobe-suite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.adobe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: image.adobe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: null\n- host: lr.adobe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: adobe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: adobe.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/security/adobe-suite-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Ai
- Analytics
- Automation
- Commerce
- Creative
- Design
- Documents
- Experience
- Marketing
- Personalization
- Video
---
