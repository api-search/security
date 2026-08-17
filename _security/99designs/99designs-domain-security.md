---
api_specs:
- filename: 99designs-briefs-api-openapi.yml
  format: yaml
  label: 99designs Briefs API
  slug: 99designs-briefs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/99designs/refs/heads/main/openapi/99designs-briefs-api-openapi.yml
- filename: 99designs-coupons-api-openapi.yml
  format: yaml
  label: 99designs Coupons API
  slug: 99designs-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/99designs/refs/heads/main/openapi/99designs-coupons-api-openapi.yml
- filename: 99designs-designers-api-openapi.yml
  format: yaml
  label: 99designs Designers API
  slug: 99designs-designers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/99designs/refs/heads/main/openapi/99designs-designers-api-openapi.yml
- filename: 99designs-products-api-openapi.yml
  format: yaml
  label: 99designs Products API
  slug: 99designs-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/99designs/refs/heads/main/openapi/99designs-products-api-openapi.yml
- filename: 99designs-orders-api-openapi.yml
  format: yaml
  label: 99designs Orders API
  slug: 99designs-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/99designs/refs/heads/main/openapi/99designs-orders-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 99designs.com
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: www.99designs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: api.99designs.com
  hsts: null
  https: true
  note: 'The probe reads the host root, which returns 404 with no HSTS header. Responses from the API itself (e.g. GET /resources/v1/designers) DO carry strict-transport-security: max-age=120; includeSubDomains — a 2-minute max-age, far below the 31536000 the website host sets. Observed 2026-08-13.'
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: 99Designs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 99designs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 99designs
provider_slug: 99designs
slug: 99designs-domain-security
source_filename: 99designs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.99designs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.99designs.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: null\n  note: >-\n    The probe reads the host root, which returns 404 with no HSTS header. Responses\n    from the API itself (e.g. GET /resources/v1/designers) DO carry\n    strict-transport-security: max-age=120; includeSubDomains — a 2-minute max-age,\n    far below the 31536000 the website host sets. Observed 2026-08-13.\ndomains:\n- domain: 99designs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/99designs/refs/heads/main/security/99designs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Media
- Design
- Marketplace
- Creative
- Freelance
- Graphic Design
- Branding
---
