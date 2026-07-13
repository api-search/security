---
api_specs:
- filename: fiserv-commercehub-openapi.yml
  format: yaml
  label: Fiserv CommerceHub API
  slug: commercehub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiserv/refs/heads/main/openapi/fiserv-commercehub-openapi.yml
- filename: fiserv-cardpointe-gateway-openapi.yml
  format: yaml
  label: Fiserv CardPointe Gateway API
  slug: cardpointe-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiserv/refs/heads/main/openapi/fiserv-cardpointe-gateway-openapi.yml
- filename: fiserv-bankinghub-openapi.yml
  format: yaml
  label: Fiserv BankingHub API
  slug: bankinghub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiserv/refs/heads/main/openapi/fiserv-bankinghub-openapi.yml
- filename: fiserv-carddeveloper-openapi.yml
  format: yaml
  label: Fiserv CardDeveloper API
  slug: carddeveloper
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiserv/refs/heads/main/openapi/fiserv-carddeveloper-openapi.yml
- filename: fiserv-payment-events-asyncapi.yml
  format: yaml
  label: Fiserv Payment Events
  slug: payment-events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiserv/refs/heads/main/asyncapi/fiserv-payment-events-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fiserv.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: fiserv.dev
  spf: false
hosts:
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: www.fiserv.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: developer.fiserv.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  2 18:11:26 2026 GMT
  host: docs.fiserv.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fiserv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fiserv, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fiserv
provider_slug: fiserv
slug: fiserv-domain-security
source_filename: fiserv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fiserv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.fiserv.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.fiserv.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:11:26 2026 GMT\n  hsts: null\ndomains:\n- domain: fiserv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fiserv.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiserv/refs/heads/main/security/fiserv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Financial
- Payments
- Wealth Management
- Fortune 500
---
