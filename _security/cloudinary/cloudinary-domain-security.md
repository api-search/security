---
api_specs:
- filename: cloudinary-openapi.yml
  format: yaml
  label: Cloudinary Upload API
  slug: upload
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudinary/refs/heads/main/openapi/cloudinary-openapi.yml
- filename: cloudinary-notifications-asyncapi.yml
  format: yaml
  label: Cloudinary Notifications and Webhooks
  slug: notifications
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudinary/refs/heads/main/asyncapi/cloudinary-notifications-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cloudinary.com
  spf: true
hosts:
- cert_expires: Dec  2 19:39:12 2026 GMT
  host: cloudinary.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 16:30:26 2026 GMT
  host: console.cloudinary.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: api.cloudinary.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cloudinary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloudinary, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cloudinary
provider_slug: cloudinary
slug: cloudinary-domain-security
source_filename: cloudinary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloudinary.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 19:39:12 2026 GMT\n  hsts: false\n- host: console.cloudinary.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 25 16:30:26 2026 GMT\n  hsts: false\n- host: api.cloudinary.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cloudinary.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudinary/refs/heads/main/security/cloudinary-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Asset Management
- Digital Asset Management
- Image Processing
- Image Transformation
- Media
- SaaS
- Video Processing
---
