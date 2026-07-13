---
api_specs:
- filename: yelp-openapi.yml
  format: yaml
  label: Yelp Fusion API
  slug: yelp-fusion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yelp/refs/heads/main/openapi/yelp-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: yelp.com
  spf: true
hosts:
- cert_expires: Sep 30 20:29:47 2026 GMT
  host: docs.developer.yelp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: api.yelp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yelp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yelp, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Yelp
provider_slug: yelp
slug: yelp-domain-security
source_filename: yelp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.developer.yelp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 20:29:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.yelp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yelp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yelp/refs/heads/main/security/yelp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Local Search
- Reviews
- Business Data
- Location
---
