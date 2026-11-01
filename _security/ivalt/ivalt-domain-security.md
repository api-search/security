---
api_specs:
- filename: ivalt-openapi-generated.yml
  format: yaml
  label: iVALT API
  slug: ivalt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivalt/openapi/_ae-authored/ivalt-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ivalt.com
  spf: true
hosts:
- cert_expires: Dec  5 10:12:20 2026 GMT
  host: ivalt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ivalt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iVALT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: iVALT
provider_slug: ivalt
slug: ivalt-domain-security
source_filename: ivalt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ivalt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 10:12:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ivalt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ivalt/security/ivalt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Identity
- Security
- HumanAuthority
---
