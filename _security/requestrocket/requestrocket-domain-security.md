---
api_specs:
- filename: requestrocket-requestrocket-api-api-openapi.yml
  format: yaml
  label: RequestRocket API
  slug: requestrocket-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/requestrocket/openapi/requestrocket-requestrocket-api-api-openapi.yml
- filename: requestrocket-openapi-generated.yml
  format: yaml
  label: RequestRocket API
  slug: requestrocket-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/requestrocket/openapi/_ae-authored/requestrocket-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: requestrocket.com
  spf: true
hosts:
- cert_expires: Apr  5 23:59:59 2027 GMT
  host: requestrocket.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Requestrocket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RequestRocket, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RequestRocket
provider_slug: requestrocket
slug: requestrocket-domain-security
source_filename: requestrocket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: requestrocket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: requestrocket.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/requestrocket/security/requestrocket-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Security
- Software-as-a-Service
- Access Control
---
