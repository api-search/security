---
api_specs:
- filename: businessportal-gr-companies-api-openapi.yml
  format: yaml
  label: GEMI General Commercial Registry (Greece) Companies API
  slug: businessportal-gr-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessportal-gr/openapi/businessportal-gr-companies-api-openapi.yml
- filename: businessportal-gr-companydocuments-api-openapi.yml
  format: yaml
  label: GEMI General Commercial Registry (Greece) Company Documents API
  slug: businessportal-gr-companydocuments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessportal-gr/openapi/businessportal-gr-companydocuments-api-openapi.yml
- filename: businessportal-gr-downloadfile-api-openapi.yml
  format: yaml
  label: GEMI General Commercial Registry (Greece) Download File API
  slug: businessportal-gr-downloadfile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessportal-gr/openapi/businessportal-gr-downloadfile-api-openapi.yml
- filename: businessportal-gr-metadata-api-openapi.yml
  format: yaml
  label: GEMI General Commercial Registry (Greece) Metadata API
  slug: businessportal-gr-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessportal-gr/openapi/businessportal-gr-metadata-api-openapi.yml
- filename: businessportal-gr-misc-api-openapi.yml
  format: yaml
  label: GEMI General Commercial Registry (Greece) Misc API
  slug: businessportal-gr-misc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessportal-gr/openapi/businessportal-gr-misc-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: businessportal.gr
  spf: true
hosts:
- cert_expires: Feb  9 11:45:16 2027 GMT
  host: www.businessportal.gr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GEMI General Commercial Registry (Greece) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GEMI General Commercial Registry (Greece), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GEMI General Commercial Registry (Greece)
provider_slug: businessportal-gr
slug: businessportal-gr-domain-security
source_filename: businessportal-gr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.businessportal.gr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 11:45:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: businessportal.gr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/businessportal-gr/security/businessportal-gr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Business Registry
- Government
- Open Data
- Greece
- Company Data
- Public Sector
---
