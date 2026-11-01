---
api_specs:
- filename: cincel-openapi-generated.yml
  format: yaml
  label: CINCEL API
  slug: cincel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cincel/openapi/_ae-authored/cincel-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cincel.digital
  spf: true
hosts:
- cert_expires: Dec 31 01:50:09 2026 GMT
  host: cincel.digital
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cincel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CINCEL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CINCEL
provider_slug: cincel
slug: cincel-domain-security
source_filename: cincel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cincel.digital\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 01:50:09 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cincel.digital\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cincel/security/cincel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- DigitalSignature
- SaaS
- LatinAmerica
- Compliance
---
