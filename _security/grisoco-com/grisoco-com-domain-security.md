---
api_specs:
- filename: grisoco-com-check-api-openapi.yml
  format: yaml
  label: Grisoco AI Check API
  slug: grisoco-com-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grisoco-com/openapi/grisoco-com-check-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: grisoco.com
  spf: true
hosts:
- cert_expires: Jan 27 21:35:58 2027 GMT
  host: grisoco.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Grisoco AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grisoco AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Grisoco AI
provider_slug: grisoco-com
slug: grisoco-com-domain-security
source_filename: grisoco-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grisoco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 21:35:58 2027 GMT\n  hsts: null\ndomains:\n- domain: grisoco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/grisoco-com/security/grisoco-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Smart-contract
- Artificial Intelligence
- Security
- Audit
- Payments
---
