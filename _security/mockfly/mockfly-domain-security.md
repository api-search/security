---
api_specs:
- filename: mockfly-openapi.json
  format: json
  label: Mockfly Public API
  slug: mockfly-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mockfly/openapi/mockfly-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mockfly.dev
  spf: true
hosts:
- cert_expires: Dec 27 10:34:07 2026 GMT
  host: mockfly.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 18:03:22 2026 GMT
  host: api.mockfly.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Mockfly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mockfly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mockfly
provider_slug: mockfly
slug: mockfly-domain-security
source_filename: mockfly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mockfly.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 10:34:07 2026 GMT\n  hsts: false\n- host: api.mockfly.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 18:03:22 2026 GMT\n  hsts: null\ndomains:\n- domain: mockfly.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mockfly/security/mockfly-domain-security.yml
summary_line: TLSv1.3
tags:
- API Platform
- Mock APIs
- Developer Tools
- Testing
- CI/CD Integration
---
