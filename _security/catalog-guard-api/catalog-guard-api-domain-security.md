---
api_specs:
- filename: catalog-guard-api-catalog-api-openapi.yml
  format: yaml
  label: Catalog Guard API Catalog API
  slug: catalog-guard-api-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/catalog-guard-api/refs/heads/main/openapi/catalog-guard-api-catalog-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workers.dev
  note: workers.dev is Cloudflare's shared Workers subdomain, not a domain Catalog Guard controls. The SPF/DMARC records above are Cloudflare's and say nothing about this provider's own email or DNS posture. Catalog Guard publishes no apex domain of its own; the entire public surface is a workers.dev subdomain (catalogguard.noahcortezj-c.workers.dev), which also means no /.well-known/ document, security.txt, CAA policy or DNSSEC can be attributed to the provider.
  spf: true
hosts:
- api_route_headers:
    cache_control: no-store
    content_security_policy: default-src 'none'; frame-ancestors 'none'; base-uri 'none'
    cross_origin_resource_policy: same-origin
    referrer_policy: no-referrer
    strict_transport_security: max-age=31536000; includeSubDomains
    x_content_type_options: nosniff
    x_frame_options: DENY
  cert_expires: Oct 10 19:05:08 2026 GMT
  host: catalogguard.noahcortezj-c.workers.dev
  hsts: false
  https: true
  note: 'HSTS is absent on the HTML routes (GET / returns no Strict-Transport-Security, no CSP, no X-Frame-Options). The JSON API routes DO set them: GET /api/v1/catalog/health and POST /api/v1/catalog/check return strict-transport-security: max-age=31536000; includeSubDomains, plus content-security-policy: default-src ''none''; frame-ancestors ''none''; base-uri ''none'', x-content-type-options: nosniff, x-frame-options: DENY, referrer-policy: no-referrer, cross-origin-resource-policy: same-origin, cache-control: no-store and x-robots-tag: noindex, nofollow. The security-header posture is therefore strong on the API surface and absent on the marketing/docs surface.'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Catalog Guard Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Catalog Guard API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Catalog Guard API
provider_slug: catalog-guard-api
slug: catalog-guard-api-domain-security
source_filename: catalog-guard-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: catalogguard.noahcortezj-c.workers.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 19:05:08 2026 GMT\n  hsts: false\n  note: >-\n    HSTS is absent on the HTML routes (GET / returns no Strict-Transport-Security,\n    no CSP, no X-Frame-Options). The JSON API routes DO set them: GET\n    /api/v1/catalog/health and POST /api/v1/catalog/check return\n    strict-transport-security: max-age=31536000; includeSubDomains, plus\n    content-security-policy: default-src 'none'; frame-ancestors 'none'; base-uri 'none',\n    x-content-type-options: nosniff, x-frame-options: DENY, referrer-policy: no-referrer,\n    cross-origin-resource-policy: same-origin, cache-control: no-store and\n    x-robots-tag: noindex, nofollow. The security-header posture is therefore\n    strong on the API surface and absent on the marketing/docs surface.\n  api_route_headers:\n\
  \    strict_transport_security: max-age=31536000; includeSubDomains\n    content_security_policy: \"default-src 'none'; frame-ancestors 'none'; base-uri 'none'\"\n    x_content_type_options: nosniff\n    x_frame_options: DENY\n    referrer_policy: no-referrer\n    cross_origin_resource_policy: same-origin\n    cache_control: no-store\ndomains:\n- domain: workers.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  note: >-\n    workers.dev is Cloudflare's shared Workers subdomain, not a domain Catalog Guard\n    controls. The SPF/DMARC records above are Cloudflare's and say nothing about this\n    provider's own email or DNS posture. Catalog Guard publishes no apex domain of its\n    own; the entire public surface is a workers.dev subdomain\n    (catalogguard.noahcortezj-c.workers.dev), which also means no /.well-known/ document,\n    security.txt, CAA policy or DNSSEC can be attributed to the provider.\nx-evidence:\n  fetched: '2026-08-09'\n  api_header_probe:\
  \ https://catalogguard.noahcortezj-c.workers.dev/api/v1/catalog/health\n  html_header_probe: https://catalogguard.noahcortezj-c.workers.dev/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catalog-guard-api/refs/heads/main/security/catalog-guard-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- E-Commerce
- catalog-validation
- Shopify
- Data Quality
- csv-validation
- product-data-qa
- data-preflight
- Data Validation
- Retail
---
