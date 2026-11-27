---
api_specs:
- filename: doorsetbook-com-api-openapi.json
  format: json
  label: DoorsetBook API API
  slug: doorsetbook-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doorsetbook-com/openapi/_original/doorsetbook-com-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: doorsetbook.com
  spf: true
hosts:
- cert_expires: Jan 30 11:34:35 2027 GMT
  host: doorsetbook.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DoorsetBook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DoorsetBook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DoorsetBook
provider_slug: doorsetbook-com
slug: doorsetbook-com-domain-security
source_filename: doorsetbook-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doorsetbook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 11:34:35 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: doorsetbook.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/doorsetbook-com/security/doorsetbook-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- FireDoors
- Inspection
- Tools
- Property Management
- Compliance
---
