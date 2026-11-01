---
api_specs:
- filename: digitalpipe-net-openapi-generated.yml
  format: yaml
  label: digitalpipe-net API
  slug: digitalpipe-net-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/digitalpipe-net/openapi/_ae-authored/digitalpipe-net-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: digitalpipe.net
  spf: true
hosts:
- cert_expires: Jan  2 19:30:11 2027 GMT
  host: digitalpipe.net
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Digitalpipe Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for digitalpipe-net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: digitalpipe-net
provider_slug: digitalpipe-net
slug: digitalpipe-net-domain-security
source_filename: digitalpipe-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digitalpipe.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 19:30:11 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: digitalpipe.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/digitalpipe-net/security/digitalpipe-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- MCP
- API Management
- Security
- Cloud
---
