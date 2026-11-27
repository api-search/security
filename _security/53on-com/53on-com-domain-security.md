---
api_specs:
- filename: 53on-com-s-service-api-openapi.yml
  format: yaml
  label: 53ON S {service} API
  slug: 53on-com-s-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/53on-com/openapi/53on-com-s-service-api-openapi.yml
- filename: 53on-com-xsite-api-openapi.yml
  format: yaml
  label: 53ON Xsite API
  slug: 53on-com-xsite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/53on-com/openapi/53on-com-xsite-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 53on.com
  spf: true
hosts:
- cert_expires: Jan 26 22:45:46 2027 GMT
  host: 53on.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 53ON Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 53ON, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 53ON
provider_slug: 53on-com
slug: 53on-com-domain-security
source_filename: 53on-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 53on.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 22:45:46 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 53on.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/53on-com/security/53on-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketplace
- Directory
- Local Business
- Services
- Consumer
- Company
---
