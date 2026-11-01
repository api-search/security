---
api_specs:
- filename: requestly-openapi-generated.yml
  format: yaml
  label: Requestly API
  slug: requestly-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/requestly/openapi/_ae-authored/requestly-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: requestly.com
  spf: true
hosts:
- cert_expires: Dec 10 15:35:45 2026 GMT
  host: requestly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Requestly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Requestly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Requestly
provider_slug: requestly
slug: requestly-domain-security
source_filename: requestly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: requestly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 15:35:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: requestly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/requestly/security/requestly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API
- Platform
- Testing
- Development
- Collaboration
- Security
---
