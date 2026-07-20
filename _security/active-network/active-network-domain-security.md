---
api_specs:
- filename: active-network-activity-search-openapi.yml
  format: yaml
  label: ACTIVE Network Activity Search API v2
  slug: active-network-activity-search-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-network/refs/heads/main/openapi/active-network-activity-search-openapi.yml
- filename: active-network-campground-search-openapi.yml
  format: yaml
  label: ACTIVE Network Campground Search API
  slug: active-network-campground-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-network/refs/heads/main/openapi/active-network-campground-search-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: activenetwork.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: active.com
  spf: true
hosts:
- cert_expires: Sep 12 10:03:21 2026 GMT
  host: www.activenetwork.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: developer.active.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: api.amp.active.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Active Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Active Network, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Active Network
provider_slug: active-network
slug: active-network-domain-security
source_filename: active-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.activenetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 10:03:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.active.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: false\n- host: api.amp.active.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: activenetwork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: active.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/active-network/refs/heads/main/security/active-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Events
- Registration
- Recreation
- Activities
- Sports
- Camping
- Search
- Ticketing
---
