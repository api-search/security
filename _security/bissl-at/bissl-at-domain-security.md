---
api_specs:
- filename: bissl-at-dishes-api-openapi.yml
  format: yaml
  label: bissl-at Dishes API
  slug: bissl-at-dishes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bissl-at/openapi/bissl-at-dishes-api-openapi.yml
- filename: bissl-at-lunch-api-openapi.yml
  format: yaml
  label: bissl-at Lunch API
  slug: bissl-at-lunch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bissl-at/openapi/bissl-at-lunch-api-openapi.yml
- filename: bissl-at-venues-api-openapi.yml
  format: yaml
  label: bissl-at Venues API
  slug: bissl-at-venues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bissl-at/openapi/bissl-at-venues-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bissl.at
  spf: true
hosts:
- cert_expires: Jan  8 21:24:36 2027 GMT
  host: bissl.at
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: bissl-at Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bissl-at, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: bissl-at
provider_slug: bissl-at
slug: bissl-at-domain-security
source_filename: bissl-at-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bissl.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 21:24:36 2027 GMT\n  hsts: false\ndomains:\n- domain: bissl.at\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bissl-at/security/bissl-at-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
