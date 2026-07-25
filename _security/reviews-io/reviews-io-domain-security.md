---
api_specs:
- filename: reviews-io-company-reviews-api-openapi.yml
  format: yaml
  label: REVIEWS.io Company Reviews API
  slug: reviews-io-company-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/openapi/reviews-io-company-reviews-api-openapi.yml
- filename: reviews-io-invitations-api-openapi.yml
  format: yaml
  label: REVIEWS.io Invitations API
  slug: reviews-io-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/openapi/reviews-io-invitations-api-openapi.yml
- filename: reviews-io-product-reviews-api-openapi.yml
  format: yaml
  label: REVIEWS.io Product Reviews API
  slug: reviews-io-product-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/openapi/reviews-io-product-reviews-api-openapi.yml
- filename: reviews-io-questions-api-openapi.yml
  format: yaml
  label: REVIEWS.io Questions API
  slug: reviews-io-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/openapi/reviews-io-questions-api-openapi.yml
- filename: reviews-io-ratings-api-openapi.yml
  format: yaml
  label: REVIEWS.io Ratings API
  slug: reviews-io-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/openapi/reviews-io-ratings-api-openapi.yml
- filename: reviews-io-webhooks-api-openapi.yml
  format: yaml
  label: REVIEWS.io Webhooks API
  slug: reviews-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/openapi/reviews-io-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: reviews.io
  spf: true
hosts:
- cert_expires: Sep 30 21:12:21 2026 GMT
  host: www.reviews.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 15:00:05 2026 GMT
  host: developer.reviews.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 21:12:21 2026 GMT
  host: api.reviews.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reviews Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for REVIEWS.io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: REVIEWS.io
provider_slug: reviews-io
slug: reviews-io-domain-security
source_filename: reviews-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reviews.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:12:21 2026 GMT\n  hsts: false\n- host: developer.reviews.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 15:00:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.reviews.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:12:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reviews.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reviews-io/refs/heads/main/security/reviews-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Reviews
- UGC
- Ratings
- Reputation
- eCommerce
---
