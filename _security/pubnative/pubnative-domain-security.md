---
api_specs:
- filename: pubnative-openapi-generated.yml
  format: yaml
  label: PubNative API
  slug: pubnative-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pubnative/openapi/_ae-authored/pubnative-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: verve.com
  spf: true
hosts:
- cert_expires: Jan 10 10:58:23 2027 GMT
  host: verve.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: PubNative Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PubNative, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PubNative
provider_slug: pubnative
slug: pubnative-domain-security
source_filename: pubnative-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verve.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 10:58:23 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: verve.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/pubnative/security/pubnative-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AdTech
- Mobile
- Monetization
- Publishers
---
