---
api_specs:
- filename: t0ll-xyz-openapi-generated.yml
  format: yaml
  label: Toll API
  slug: t0ll-xyz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/t0ll-xyz/openapi/_ae-authored/t0ll-xyz-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: t0ll.xyz
  spf: true
hosts:
- cert_expires: Dec 27 18:56:56 2026 GMT
  host: t0ll.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Toll Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toll, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Toll
provider_slug: t0ll-xyz
slug: t0ll-xyz-domain-security
source_filename: t0ll-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: t0ll.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 18:56:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: t0ll.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/t0ll-xyz/security/t0ll-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Finance
- Security
- Blockchain
- API
- Agentic
---
