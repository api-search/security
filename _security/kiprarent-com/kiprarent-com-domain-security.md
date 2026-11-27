---
api_specs:
- filename: kiprarent-com-public-api-openapi.yml
  format: yaml
  label: Kipra Rent A Car Public API
  slug: kiprarent-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kiprarent-com/openapi/kiprarent-com-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kiprarent.com
  spf: true
hosts:
- cert_expires: Feb 12 05:15:40 2027 GMT
  host: kiprarent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kipra Rent A Car Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kipra Rent A Car, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kipra Rent A Car
provider_slug: kiprarent-com
slug: kiprarent-com-domain-security
source_filename: kiprarent-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kiprarent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 05:15:40 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kiprarent.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/kiprarent-com/security/kiprarent-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
