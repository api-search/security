---
api_specs:
- filename: cj-affiliate-openapi.yml
  format: yaml
  label: CJ Link Search API
  slug: cj-affiliate-link-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-openapi.yml
- filename: cj-affiliate-openapi.yml
  format: yaml
  label: CJ Advertiser Lookup API
  slug: cj-affiliate-advertiser-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-openapi.yml
- filename: cj-affiliate-openapi.yml
  format: yaml
  label: CJ Publisher Lookup API
  slug: cj-affiliate-publisher-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-openapi.yml
- filename: cj-affiliate-openapi.yml
  format: yaml
  label: CJ Product Search (Legacy) API
  slug: cj-affiliate-product-search-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazontrust.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cj.com
  spf: true
hosts:
- cert_expires: Sep 19 09:41:22 2026 GMT
  host: www.cj.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: developers.cj.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: commissions.api.cj.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cj Affiliate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CJ Affiliate, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CJ Affiliate
provider_slug: cj-affiliate
slug: cj-affiliate-domain-security
source_filename: cj-affiliate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cj.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 09:41:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.cj.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: commissions.api.cj.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cj.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/security/cj-affiliate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Affiliate Marketing
- Affiliate Network
- Commission
- Product Search
- Publisher
- Advertiser
- GraphQL
- Ecommerce
---
