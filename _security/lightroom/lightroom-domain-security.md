---
api_specs:
- filename: lightroom-services-openapi.yml
  format: yaml
  label: Lightroom Services API
  slug: lightroom-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-services-openapi.yml
- filename: lightroom-firefly-services-openapi.yml
  format: yaml
  label: Adobe Lightroom API (Firefly Services)
  slug: lightroom-firefly-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-firefly-services-openapi.yml
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
- cert_expires: Aug 26 23:59:59 2026 GMT
  host: lr.adobe.io
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
name: Lightroom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adobe Lightroom, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adobe Lightroom
provider_slug: lightroom
slug: lightroom-domain-security
source_filename: lightroom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.adobe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: lr.adobe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:59:59 2026 GMT\n  hsts: null\n- host: image.adobe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: adobe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: adobe.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/security/lightroom-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
---
