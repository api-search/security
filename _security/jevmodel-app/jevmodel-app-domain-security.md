---
api_specs:
- filename: jevmodel-app-openapi-generated.yml
  format: yaml
  label: JevModel API
  slug: jevmodel-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jevmodel-app/openapi/_ae-authored/jevmodel-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jevmodel.app
  spf: true
hosts:
- cert_expires: Jan 24 06:51:55 2027 GMT
  host: jevmodel.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jevmodel App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JevModel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: JevModel
provider_slug: jevmodel-app
slug: jevmodel-app-domain-security
source_filename: jevmodel-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jevmodel.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 06:51:55 2027 GMT\n  hsts: false\ndomains:\n- domain: jevmodel.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/jevmodel-app/security/jevmodel-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Decision API
- Content Moderation
- Spam Filtering
- Support Triage
- Ticket Routing
- Language Detection
- Personal Data Screening
---
