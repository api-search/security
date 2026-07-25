---
api_specs:
- filename: bazaarvoice-answers-api-openapi.yml
  format: yaml
  label: Bazaarvoice Answers API
  slug: bazaarvoice-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-answers-api-openapi.yml
- filename: bazaarvoice-clients-api-openapi.yml
  format: yaml
  label: Bazaarvoice Clients API
  slug: bazaarvoice-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-clients-api-openapi.yml
- filename: bazaarvoice-contributor-api-openapi.yml
  format: yaml
  label: Bazaarvoice Contributor API
  slug: bazaarvoice-contributor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-contributor-api-openapi.yml
- filename: bazaarvoice-lookahead-api-openapi.yml
  format: yaml
  label: Bazaarvoice Lookahead API
  slug: bazaarvoice-lookahead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-lookahead-api-openapi.yml
- filename: bazaarvoice-questions-api-openapi.yml
  format: yaml
  label: Bazaarvoice Questions API
  slug: bazaarvoice-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-questions-api-openapi.yml
- filename: bazaarvoice-reviews-api-openapi.yml
  format: yaml
  label: Bazaarvoice Reviews API
  slug: bazaarvoice-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-reviews-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bazaarvoice.com
  spf: true
hosts:
- host: content-search.eu-west-1a.bosun.qa.bazaarvoice.com
  https: false
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: seo-stg.bazaarvoice.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: seo.bazaarvoice.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bazaarvoice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bazaarvoice, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bazaarvoice
provider_slug: bazaarvoice
slug: bazaarvoice-domain-security
source_filename: bazaarvoice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: content-search.eu-west-1a.bosun.qa.bazaarvoice.com\n  https: false\n- host: seo-stg.bazaarvoice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: null\n- host: seo.bazaarvoice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bazaarvoice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/security/bazaarvoice-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Reviews
- Ratings
- User Generated Content
- Retail
- eCommerce
- Product Reviews
- Syndication
- Social Commerce
- SEO
---
