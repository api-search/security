---
api_specs:
- filename: consequential-io-openapi-generated.yml
  format: yaml
  label: Consequential API
  slug: consequential-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/consequential-io/openapi/_ae-authored/consequential-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: consequential.io
  spf: true
hosts:
- cert_expires: Dec 16 18:34:16 2026 GMT
  host: consequential.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Consequential Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Consequential, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Consequential
provider_slug: consequential-io
slug: consequential-io-domain-security
source_filename: consequential-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: consequential.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 18:34:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: consequential.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/consequential-io/security/consequential-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Advertising
- E-Commerce
- Revenue Intelligence
- Software-as-a-Service
---
