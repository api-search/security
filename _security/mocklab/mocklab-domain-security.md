---
api_specs:
- filename: mocklab-openapi-generated.yml
  format: yaml
  label: MockLab API
  slug: mocklab-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mocklab/openapi/_ae-authored/mocklab-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mocklab.io
  spf: true
hosts:
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: mocklab.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mocklab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MockLab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MockLab
provider_slug: mocklab
slug: mocklab-domain-security
source_filename: mocklab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mocklab.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: mocklab.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mocklab/security/mocklab-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Mocking
- Environment Simulation
- Testing
- Fintech
- Service Virtualization
- Cloud Service
---
