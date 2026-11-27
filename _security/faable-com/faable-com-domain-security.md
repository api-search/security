---
api_specs:
- filename: faable-com-openapi-generated.yml
  format: yaml
  label: Faable API
  slug: faable-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faable-com/openapi/_ae-authored/faable-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: faable.com
  spf: true
hosts:
- cert_expires: Jan 24 12:03:26 2027 GMT
  host: faable.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Faable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Faable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Faable
provider_slug: faable-com
slug: faable-com-domain-security
source_filename: faable-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: faable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 12:03:26 2027 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: faable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/faable-com/security/faable-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- ZeroOps
- Hosting
- Identity
- GDPR
- Software-as-a-Service
---
