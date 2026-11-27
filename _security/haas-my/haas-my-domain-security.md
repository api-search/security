---
api_specs:
- filename: haas-my-openapi-generated.yml
  format: yaml
  label: Haas.my API
  slug: haas-my-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/haas-my/openapi/_ae-authored/haas-my-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: haas.my
  spf: false
hosts:
- cert_expires: Jan 13 21:41:56 2027 GMT
  host: haas.my
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Haas.my Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Haas.my, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Haas.my
provider_slug: haas-my
slug: haas-my-domain-security
source_filename: haas-my-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: haas.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 21:41:56 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: haas.my\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/haas-my/security/haas-my-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Human-as-a-Service
- AI Integration
- Marketplace
---
