---
api_specs:
- filename: judge-me-openapi.yml
  format: yaml
  label: Judge.me Reviews API
  slug: judge-me-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/openapi/judge-me-openapi.yml
- filename: judge-me-openapi.yml
  format: yaml
  label: Judge.me Reviewers API
  slug: judge-me-reviewers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/openapi/judge-me-openapi.yml
- filename: judge-me-openapi.yml
  format: yaml
  label: Judge.me Products API
  slug: judge-me-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/openapi/judge-me-openapi.yml
- filename: judge-me-openapi.yml
  format: yaml
  label: Judge.me Widgets API
  slug: judge-me-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/openapi/judge-me-openapi.yml
- filename: judge-me-openapi.yml
  format: yaml
  label: Judge.me OAuth API
  slug: judge-me-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/openapi/judge-me-openapi.yml
- filename: judge-me-openapi.yml
  format: yaml
  label: Judge.me Webhooks API
  slug: judge-me-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/openapi/judge-me-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: judge.me
  spf: true
hosts:
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: judge.me
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Judge Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Judge.me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Judge.me
provider_slug: judge-me
slug: judge-me-domain-security
source_filename: judge-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: judge.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: judge.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/judge-me/refs/heads/main/security/judge-me-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Reviews
- E-commerce
- Shopify
- Ratings
- Social Proof
---
