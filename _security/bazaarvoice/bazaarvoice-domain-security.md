---
api_specs:
- filename: bazaarvoice-content-search-openapi.json
  format: json
  label: Bazaarvoice Content Search API
  slug: bazaarvoice-content-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bazaarvoice/refs/heads/main/openapi/bazaarvoice-content-search-openapi.json
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
