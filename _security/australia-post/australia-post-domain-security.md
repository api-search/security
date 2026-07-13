---
api_specs:
- filename: locations-openapi.json
  format: json
  label: Australia Post Locations API
  slug: locations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australia-post/refs/heads/main/openapi/locations-openapi.json
- filename: delivery-partner-openapi.json
  format: json
  label: Australia Post Delivery Partner API
  slug: delivery-partner
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australia-post/refs/heads/main/openapi/delivery-partner-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: auspost.com.au
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: auspost.com.au
  hsts: true
  hsts_max_age: 15552001
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: digitalapi.auspost.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: developers.auspost.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Australia Post Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Australia Post, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Australia Post
provider_slug: australia-post
slug: australia-post-domain-security
source_filename: australia-post-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: auspost.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552001\n- host: digitalapi.auspost.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\n- host: developers.auspost.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: auspost.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australia-post/refs/heads/main/security/australia-post-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Address Validation
- Click and Collect
- Delivery
- E-Commerce
- Labels
- Locations
- Logistics
- Parcel Locker
- Postal
- Postage
- Shipping
- Tracking
---
