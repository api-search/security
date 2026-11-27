---
api_specs:
- filename: netapi-com-free-datasets-api-openapi.yml
  format: yaml
  label: NetAPI Telecom Free Datasets API
  slug: netapi-com-free-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/netapi-com/openapi/netapi-com-free-datasets-api-openapi.yml
- filename: netapi-com-json-api-api-openapi.yml
  format: yaml
  label: NetAPI Telecom JSON API
  slug: netapi-com-json-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/netapi-com/openapi/netapi-com-json-api-api-openapi.yml
- filename: netapi-com-reference-api-openapi.yml
  format: yaml
  label: NetAPI Telecom Reference API
  slug: netapi-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/netapi-com/openapi/netapi-com-reference-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: netapi.com
  spf: true
hosts:
- cert_expires: Dec 26 15:33:27 2026 GMT
  host: netapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NetAPI Telecom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NetAPI Telecom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NetAPI Telecom
provider_slug: netapi-com
slug: netapi-com-domain-security
source_filename: netapi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: netapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 15:33:27 2026 GMT\n  hsts: false\ndomains:\n- domain: netapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/netapi-com/security/netapi-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Domain Lists
- DNS Data
- WHOIS
- Threat Intelligence
- Data Feed
---
