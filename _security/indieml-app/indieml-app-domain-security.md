---
api_specs:
- filename: indieml-app-keys-api-openapi.yml
  format: yaml
  label: indieml-app Keys API
  slug: indieml-app-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indieml-app/openapi/indieml-app-keys-api-openapi.yml
- filename: indieml-app-score-api-openapi.yml
  format: yaml
  label: indieml-app Score API
  slug: indieml-app-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indieml-app/openapi/indieml-app-score-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: indieml.app
  spf: true
hosts:
- cert_expires: Jan 25 17:42:40 2027 GMT
  host: indieml.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Indieml App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for indieml-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: indieml-app
provider_slug: indieml-app
slug: indieml-app-domain-security
source_filename: indieml-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: indieml.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 17:42:40 2027 GMT\n  hsts: false\ndomains:\n- domain: indieml.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/indieml-app/security/indieml-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- NLP
- Text-Analysis
- Machine-Learning
- API
---
