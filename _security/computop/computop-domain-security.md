---
api_specs:
- filename: computop-openapi-generated.yml
  format: yaml
  label: Computop API
  slug: computop-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/computop/openapi/_ae-authored/computop-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: computop.com
  spf: true
hosts:
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: computop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Computop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Computop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Computop
provider_slug: computop
slug: computop-domain-security
source_filename: computop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: computop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: computop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/computop/security/computop-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- FinTech
- E-commerce
- Germany
- SaaS
---
