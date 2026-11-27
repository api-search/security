---
api_specs:
- filename: cafedev-co-companies-api-openapi.yml
  format: yaml
  label: CafeDev Companies API
  slug: cafedev-co-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cafedev-co/openapi/cafedev-co-companies-api-openapi.yml
- filename: cafedev-co-jobs-api-openapi.yml
  format: yaml
  label: CafeDev Jobs API
  slug: cafedev-co-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cafedev-co/openapi/cafedev-co-jobs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cafedev.co
  spf: true
hosts:
- cert_expires: Dec 30 08:28:19 2026 GMT
  host: cafedev.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CafeDev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CafeDev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CafeDev
provider_slug: cafedev-co
slug: cafedev-co-domain-security
source_filename: cafedev-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cafedev.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 08:28:19 2026 GMT\n  hsts: false\ndomains:\n- domain: cafedev.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cafedev-co/security/cafedev-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Technology
- Job
- Latin America
- Aggregator
- Free
---
