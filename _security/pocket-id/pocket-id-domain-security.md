---
api_specs:
- filename: pocket-id-openapi-generated.yml
  format: yaml
  label: Pocket ID API
  slug: pocket-id-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pocket-id/openapi/_ae-authored/pocket-id-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pocket-id.org
  spf: true
hosts:
- cert_expires: Jan 15 05:54:30 2027 GMT
  host: pocket-id.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pocket Id Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pocket ID, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pocket ID
provider_slug: pocket-id
slug: pocket-id-domain-security
source_filename: pocket-id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pocket-id.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 05:54:30 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pocket-id.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/pocket-id/security/pocket-id-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Identity
- OpenID Connect
- OAuth2
- Self-Hosted
---
