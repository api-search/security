---
api_specs:
- filename: stubhub-account-openapi.yml
  format: yaml
  label: StubHub Account API
  slug: stubhub-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-account-openapi.yml
- filename: stubhub-catalog-openapi.yml
  format: yaml
  label: StubHub Catalog API
  slug: stubhub-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-catalog-openapi.yml
- filename: stubhub-inventory-openapi.yml
  format: yaml
  label: StubHub Inventory API
  slug: stubhub-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-inventory-openapi.yml
- filename: stubhub-sales-openapi.yml
  format: yaml
  label: StubHub Sales API
  slug: stubhub-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-sales-openapi.yml
- filename: stubhub-webhooks-openapi.yml
  format: yaml
  label: StubHub Webhooks API
  slug: stubhub-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-webhooks-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stubhub.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: stubhub.net
  spf: false
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: www.stubhub.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: api.stubhub.net
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: sandbox.api.stubhub.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stubhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StubHub, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: StubHub
provider_slug: stubhub
slug: stubhub-domain-security
source_filename: stubhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stubhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stubhub.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\n- host: sandbox.api.stubhub.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: stubhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: stubhub.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/security/stubhub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplaces
- Tickets
- Events
- Ticketing
- Live Events
- Secondary Market
- E-commerce
- Sports
- Concerts
---
