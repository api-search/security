---
api_specs:
- filename: parkypass-com-live-api-openapi.yml
  format: yaml
  label: Parky Live API
  slug: parkypass-com-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parkypass-com/openapi/parkypass-com-live-api-openapi.yml
- filename: parkypass-com-meta-api-openapi.yml
  format: yaml
  label: Parky Meta API
  slug: parkypass-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parkypass-com/openapi/parkypass-com-meta-api-openapi.yml
- filename: parkypass-com-parks-api-openapi.yml
  format: yaml
  label: Parky Parks API
  slug: parkypass-com-parks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parkypass-com/openapi/parkypass-com-parks-api-openapi.yml
- filename: parkypass-com-resorts-api-openapi.yml
  format: yaml
  label: Parky Resorts API
  slug: parkypass-com-resorts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parkypass-com/openapi/parkypass-com-resorts-api-openapi.yml
- filename: parkypass-com-rides-api-openapi.yml
  format: yaml
  label: Parky Rides API
  slug: parkypass-com-rides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parkypass-com/openapi/parkypass-com-rides-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: parkypass.com
  spf: true
hosts:
- cert_expires: Feb  8 06:47:43 2027 GMT
  host: parkypass.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Parky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parky, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Parky
provider_slug: parkypass-com
slug: parkypass-com-domain-security
source_filename: parkypass-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parkypass.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 06:47:43 2027 GMT\n  hsts: false\ndomains:\n- domain: parkypass.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/parkypass-com/security/parkypass-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- ThemePark
- Mobile App
- Travel
- Disney
- Universal
---
