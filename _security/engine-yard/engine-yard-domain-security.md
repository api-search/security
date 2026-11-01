---
api_specs:
- filename: engine-yard-openapi-generated.yml
  format: yaml
  label: Engine Yard API
  slug: engine-yard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engine-yard/openapi/_ae-authored/engine-yard-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: engineyard.com
  spf: true
hosts:
- cert_expires: Dec 20 12:24:44 2026 GMT
  host: www.engineyard.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Engine Yard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Engine Yard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Engine Yard
provider_slug: engine-yard
slug: engine-yard-domain-security
source_filename: engine-yard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.engineyard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 12:24:44 2026 GMT\n  hsts: false\ndomains:\n- domain: engineyard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/engine-yard/security/engine-yard-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- PaaS
- Ruby
- Rails
- CloudHosting
---
