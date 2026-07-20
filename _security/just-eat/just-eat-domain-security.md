---
api_specs:
- filename: just-eat-uk-openapi-original.json
  format: json
  label: Just Eat UK API
  slug: just-eat-uk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/just-eat/refs/heads/main/openapi/just-eat-uk-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: just-eat.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: just-eat.io
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: www.just-eat.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  1 04:57:33 2026 GMT
  host: uk.api.just-eat.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 06:05:52 2026 GMT
  host: i18n.api.just-eat.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Just Eat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Just Eat, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Just Eat
provider_slug: just-eat
slug: just-eat-domain-security
source_filename: just-eat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.just-eat.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\n- host: uk.api.just-eat.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:57:33 2026 GMT\n  hsts: null\n- host: i18n.api.just-eat.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 06:05:52 2026 GMT\n  hsts: null\ndomains:\n- domain: just-eat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: just-eat.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/just-eat/refs/heads/main/security/just-eat-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Food Delivery
- Restaurants
- Marketplace
- Logistics
- Orders
- Delivery
- Point of Sale
- E-commerce
---
