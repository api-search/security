---
api_specs:
- filename: highway-com-openapi-generated.yml
  format: yaml
  label: Highway API
  slug: highway-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/highway-com/openapi/_ae-authored/highway-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: highway.com
  spf: true
hosts:
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: highway.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Highway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Highway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Highway
provider_slug: highway-com
slug: highway-com-domain-security
source_filename: highway-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: highway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: highway.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/highway-com/security/highway-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Carrier Identity
- Freight Brokers
- 3PL
- Trusted Freight Exchange
---
