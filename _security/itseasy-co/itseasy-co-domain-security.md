---
api_specs:
- filename: itseasy-co-core-openapi-generated.yml
  format: yaml
  label: Easy core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itseasy-co/openapi/_ae-authored/itseasy-co-core-openapi-generated.yml
- filename: itseasy-co-reference-openapi-generated.yml
  format: yaml
  label: Easy reference API
  slug: reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itseasy-co/openapi/_ae-authored/itseasy-co-reference-openapi-generated.yml
- filename: itseasy-co-sdks-openapi-generated.yml
  format: yaml
  label: Easy SDKs API
  slug: sdks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itseasy-co/openapi/_ae-authored/itseasy-co-sdks-openapi-generated.yml
- filename: itseasy-co-treasury-openapi-generated.yml
  format: yaml
  label: Easy Treasury API
  slug: treasury-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itseasy-co/openapi/_ae-authored/itseasy-co-treasury-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: itseasy.co
  spf: true
hosts:
- cert_expires: Jan  1 21:22:18 2027 GMT
  host: itseasy.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Easy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Easy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Easy
provider_slug: itseasy-co
slug: itseasy-co-domain-security
source_filename: itseasy-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: itseasy.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 21:22:18 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: itseasy.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/itseasy-co/security/itseasy-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Processor
- Self-Custody
- Cashback
- Invoicing
- Subscription
- Analytics
---
