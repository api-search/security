---
api_specs:
- filename: culqi-3ds-api-openapi.yml
  format: yaml
  label: Culqi 3DS API
  slug: culqi-3ds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-3ds-api-openapi.yml
- filename: culqi-cards-api-openapi.yml
  format: yaml
  label: Culqi Cards API
  slug: culqi-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-cards-api-openapi.yml
- filename: culqi-charges-api-openapi.yml
  format: yaml
  label: Culqi Charges API
  slug: culqi-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-charges-api-openapi.yml
- filename: culqi-customers-api-openapi.yml
  format: yaml
  label: Culqi Customers API
  slug: culqi-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-customers-api-openapi.yml
- filename: culqi-events-api-openapi.yml
  format: yaml
  label: Culqi Events API
  slug: culqi-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-events-api-openapi.yml
- filename: culqi-iins-api-openapi.yml
  format: yaml
  label: Culqi Iins API
  slug: culqi-iins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-iins-api-openapi.yml
- filename: culqi-orders-api-openapi.yml
  format: yaml
  label: Culqi Orders API
  slug: culqi-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-orders-api-openapi.yml
- filename: culqi-plans-api-openapi.yml
  format: yaml
  label: Culqi Plans API
  slug: culqi-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-plans-api-openapi.yml
- filename: culqi-refunds-api-openapi.yml
  format: yaml
  label: Culqi Refunds API
  slug: culqi-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-refunds-api-openapi.yml
- filename: culqi-subscriptions-api-openapi.yml
  format: yaml
  label: Culqi Subscriptions API
  slug: culqi-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-subscriptions-api-openapi.yml
- filename: culqi-tokens-api-openapi.yml
  format: yaml
  label: Culqi Tokens API
  slug: culqi-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-tokens-api-openapi.yml
- filename: culqi-transfers-api-openapi.yml
  format: yaml
  label: Culqi Transfers API
  slug: culqi-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-transfers-api-openapi.yml
description: ''
domains:
- caa: []
  caa_note: No CAA record published for culqi.com as of the probe date.
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; rua=mailto:infosec@culqi.com; ruf=mailto:infosec@culqi.com; pct=100; fo=0:1:d:s;
  dnssec: false
  domain: culqi.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:_spf.goskope.com include:sendgrid.net include:_spf.embluemail.com include:transmail.net include:zcsend.net include:spf.zoho.com ip4:205.201.128.0/20 ip4:198.2.128.0/18 ip4:148.105.8.0/21 ~all
hosts:
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: api.culqi.com
  hsts: false
  http_status: 403
  https: true
  note: Server-side API host. Returns 403 without a valid Bearer secret key (expected).
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: secure.culqi.com
  hsts: false
  http_status: 403
  https: true
  note: PCI-scoped tokenization / 3DS confirm host. Returns 403 without a valid Bearer public key (expected).
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: culqi.com
  hsts: false
  http_status: 200
  https: true
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: docs.culqi.com
  hsts: false
  http_status: 200
  https: true
kind: domain-security
layout: security
method: probed
name: Culqi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Culqi, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Culqi
provider_slug: culqi
slug: culqi-domain-security
source_filename: culqi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts (2026-07-17)\nhosts:\n- host: api.culqi.com\n  https: true\n  http_status: 403\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: false\n  note: Server-side API host. Returns 403 without a valid Bearer secret key (expected).\n- host: secure.culqi.com\n  https: true\n  http_status: 403\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: false\n  note: PCI-scoped tokenization / 3DS confirm host. Returns 403 without a valid Bearer public key (expected).\n- host: culqi.com\n  https: true\n  http_status: 200\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: false\n- host: docs.culqi.com\n  https: true\n  http_status: 200\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: culqi.com\n  dnssec: false\n  caa: []\n  caa_note: No CAA record published for culqi.com as of the probe date.\n  spf: true\n  spf_record: >-\n    v=spf1 include:_spf.google.com include:_spf.goskope.com\
  \ include:sendgrid.net\n    include:_spf.embluemail.com include:transmail.net include:zcsend.net\n    include:spf.zoho.com ip4:205.201.128.0/20 ip4:198.2.128.0/18\n    ip4:148.105.8.0/21 ~all\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: >-\n    v=DMARC1; p=reject; rua=mailto:infosec@culqi.com; ruf=mailto:infosec@culqi.com;\n    pct=100; fo=0:1:d:s;\nnotes: >-\n  All API and web hosts serve HTTPS with valid TLS certificates. Neither the\n  API hosts nor the marketing site returned an HSTS response header on probe.\n  Email is strongly protected: SPF is published and DMARC is at p=reject with\n  aggregate/forensic reporting to infosec@culqi.com. No CAA record was found.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/security/culqi-domain-security.yml
summary_line: DMARC
tags:
- Payments
- Payment Gateway
- Fintech
- Peru
- LatAm
- Cards
- Yape
---
