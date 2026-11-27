---
api_specs:
- filename: dispola-ca-attributs-api-openapi.yml
  format: yaml
  label: Dispola Attributs API
  slug: dispola-ca-attributs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dispola-ca/openapi/dispola-ca-attributs-api-openapi.yml
- filename: dispola-ca-places-api-openapi.yml
  format: yaml
  label: Dispola Places API
  slug: dispola-ca-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dispola-ca/openapi/dispola-ca-places-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dispola.ca
  spf: true
hosts:
- cert_expires: Jan  3 02:42:50 2027 GMT
  host: dispola.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dispola Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dispola, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dispola
provider_slug: dispola-ca
slug: dispola-ca-domain-security
source_filename: dispola-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dispola.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 02:42:50 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dispola.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dispola-ca/security/dispola-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Booking
- Salon
- Clinics
- Quebec
- Healthcare
---
