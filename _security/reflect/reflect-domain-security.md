---
api_specs:
- filename: reflect-openapi.yml
  format: yaml
  label: Reflect
  slug: reflect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reflect/refs/heads/main/openapi/reflect-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reflect.run
  spf: true
hosts:
- cert_expires: Aug 22 17:09:54 2026 GMT
  host: reflect.run
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: api.reflect.run
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reflect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reflect, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Reflect
provider_slug: reflect
slug: reflect-domain-security
source_filename: reflect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reflect.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 17:09:54 2026 GMT\n  hsts: false\n- host: api.reflect.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: reflect.run\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reflect/refs/heads/main/security/reflect-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Testing
- Artificial Intelligence
- Automated Testing
- CI/CD
- End-to-End Testing
- QA
- Testing
---
