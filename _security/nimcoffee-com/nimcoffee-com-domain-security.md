---
api_specs:
- filename: nimcoffee-com-default-api-openapi.yml
  format: yaml
  label: NiM Coffee 产品 API
  slug: nimcoffee-com-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nimcoffee-com/openapi/nimcoffee-com-default-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nimcoffee.com
  spf: false
hosts:
- cert_expires: Jan 30 19:02:09 2027 GMT
  host: nimcoffee.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NiM Coffee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NiM Coffee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: NiM Coffee
provider_slug: nimcoffee-com
slug: nimcoffee-com-domain-security
source_filename: nimcoffee-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nimcoffee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 19:02:09 2027 GMT\n  hsts: false\ndomains:\n- domain: nimcoffee.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/nimcoffee-com/security/nimcoffee-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Coffee
- AI Platform
---
