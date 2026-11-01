---
api_specs:
- filename: getenroute-core-openapi-generated.yml
  format: yaml
  label: Saaras core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getenroute/openapi/_ae-authored/getenroute-core-openapi-generated.yml
- filename: getenroute-prologue-openapi-generated.yml
  format: yaml
  label: Saaras prologue API
  slug: prologue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getenroute/openapi/_ae-authored/getenroute-prologue-openapi-generated.yml
- filename: getenroute-technical-reference-openapi-generated.yml
  format: yaml
  label: Saaras Techincal Reference API
  slug: technical-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getenroute/openapi/_ae-authored/getenroute-technical-reference-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getenroute.io
  spf: false
hosts:
- cert_expires: Jan  7 02:49:56 2027 GMT
  host: getenroute.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getenroute Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saaras, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Saaras
provider_slug: getenroute
slug: getenroute-domain-security
source_filename: getenroute-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getenroute.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 02:49:56 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getenroute.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/getenroute/security/getenroute-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- API Gateway
- Kubernetes
- Service Mesh
- Cloud-Native
---
