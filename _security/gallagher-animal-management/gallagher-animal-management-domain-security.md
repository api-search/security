---
api_specs:
- filename: gallagher-animal-management-openapi-generated.yml
  format: yaml
  label: Gallagher API
  slug: gallagher-animal-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gallagher-animal-management/openapi/_ae-authored/gallagher-animal-management-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gallagher.com
  spf: true
hosts:
- cert_expires: Apr 11 23:59:59 2027 GMT
  host: gallagher.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gallagher Animal Management Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gallagher, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gallagher
provider_slug: gallagher-animal-management
slug: gallagher-animal-management-domain-security
source_filename: gallagher-animal-management-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gallagher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gallagher.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gallagher-animal-management/security/gallagher-animal-management-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Animal Management
- Electric Fencing
- Weighing
- EID
- Watering
- Security
---
