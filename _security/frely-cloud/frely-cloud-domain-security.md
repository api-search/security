---
api_specs:
- filename: frely-cloud-openapi-generated.yml
  format: yaml
  label: Frely API
  slug: frely-cloud-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frely-cloud/openapi/_ae-authored/frely-cloud-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: frely.cloud
  spf: true
hosts:
- cert_expires: Jan 31 08:10:23 2027 GMT
  host: frely.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Frely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frely, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Frely
provider_slug: frely-cloud
slug: frely-cloud-domain-security
source_filename: frely-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frely.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 08:10:23 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: frely.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/frely-cloud/security/frely-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Integration
- Computer access
---
